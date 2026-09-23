---
name: ai-reel
description: Erstellt ein komplett neues KI-Avatar-Reel mit Jennifers geklonter Stimme und Aussehen via HeyGen. Nutzen wenn Jennifer ein neues Reel will, das sie NICHT selbst aufnehmen muss ("mach mir ein neues Reel", "AI-Reel", "HeyGen-Reel").
---

# AI-Reel (HeyGen) erstellen

Erzeugt ein neues Reel, in dem Jennifer spricht und zu sehen ist, ohne dass sie aufnimmt. Nutzt ihren HeyGen-Avatar + Stimm-Klon.

## Voraussetzung (einmalig von Jennifer)
1. HeyGen-Konto + eigener Avatar (Consent-Video) + geklonte Stimme.
2. API-Key als Umgebungsvariable: `export HEYGEN_API_KEY="..."`.
3. Einmal `python3 ~/.claude/marketing/heygen_reel.py list` laufen lassen → avatar_id + voice_id ins Skript eintragen.
Wenn das noch nicht existiert: zuerst die Anleitung `~/.claude/marketing/heygen-setup.md` durchgehen.

## Standard-Ablauf (3 Schritte)
Alles läuft im Ordner `~/.claude/marketing/`. Key aus `.heygen.env` laden.

1. **Skript schreiben** (Agent `social-content` / `ghostwriter`): Hook (Sek. 1-2) → ein Gedanke → CTA. ~40-60 Sek. gesprochen. Kleines „du", keine Gedankenstriche, Marke Soul Marketing.
2. **Rendern** (HeyGen, Standard-Avatar + Standard-Stimme #2 + Tempo 0.9 sind hinterlegt):
   ```
   source ~/.claude/marketing/.heygen.env
   python3 ~/.claude/marketing/heygen_reel.py make "SKRIPTTEXT" --out ~/.claude/marketing/video-work/raw.mp4
   ```
3. **Freistellen** (rembg, ~7 Min bei 35 Sek.) auf Marken-Hintergrund:
   ```
   python3 ~/.claude/marketing/video-work/cutout_reel.py --src .../raw.mp4 --bg ~/.claude/marketing/video-work/hintergrund-soul.png --fade-start 0.60 --fade-end 0.70 --out .../cut.mp4
   ```
4. **Bunte Untertitel** (Mint/Grün/Pink) einbrennen:
   ```
   ffmpeg -y -i .../cut.mp4 -ar 16000 -ac 1 a.wav
   whisper-cli -m ~/.claude/marketing/video-work/ggml-small.bin -f a.wav -l de -ml 20 -sow -osrt -of subs
   python3 ~/.claude/marketing/video-work/burn_subs.py --src .../cut.mp4 --srt subs.srt --out ~/Desktop/reel-final.mp4
   ```
5. **Ausliefern:** fertiges mp4 an Jennifer senden, Kopie in `~/.claude/marketing/queue/`, Dashboard-Queue aktualisieren.

Standard bestätigt (2026-07-01): Avatar 1, Voice-Clone #2 (a459fcf6…), Tempo 0.9, freigestellt, bunte Untertitel.

## Ohne API-Key (Fallback)
Wenn (noch) kein Key da ist: das komplette HeyGen-fertige Paket ausgeben (Skript + On-Screen + Hintergrund-Bild + Caption). Jennifer fügt das Skript in HeyGen ein und rendert mit einem Klick.

## Themen-Ideen (aus dem Buch)
Sichtbarkeit als Dienst · der erste Schritt trotz Angst · Geld ist Energie · KI als Verbündete · alte Muster auflösen · Preis = Selbstachtung.
