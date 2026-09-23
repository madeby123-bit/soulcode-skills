---
name: untertitel
description: Erzeugt Untertitel (.srt) aus einem Video per Whisper-Transkription (Deutsch).
---

# Untertitel erzeugen

Delegiere an `video-cutter`.

## Schritte
1. Whisper pruefen/installieren: `pip3 install -q openai-whisper` (oder `brew install openai-whisper`).
2. Transkribieren: `whisper in.mp4 --language German --model small --output_format srt --output_dir .`
3. `.srt` kurz gegenlesen (Namen/Fachbegriffe korrigieren).

Ergebnis: `in.srt`. Danach optional `/untertitel-burn`.
