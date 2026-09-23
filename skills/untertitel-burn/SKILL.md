---
name: untertitel-burn
description: Brennt Untertitel im CapCut-Stil fest ins Video ein (grosse fette weisse Schrift mit Outline).
---

# Untertitel einbrennen (CapCut-Stil)

Delegiere an `video-cutter`. Voraussetzung: `.srt` vorhanden (`/untertitel`).

## Befehl
`ffmpeg -i in.mp4 -vf "subtitles=in.srt:force_style='FontName=Arial,FontSize=16,Bold=1,PrimaryColour=&H00FFFFFF,OutlineColour=&H00000000,Outline=3,Shadow=1,Alignment=2,MarginV=60'" -c:a copy out.mp4`

- Fuer 9:16-Shorts FontSize ~18-22.
- Markenfarbe statt Weiss: PrimaryColour als &H00BBGGRR Hex.

Real ausfuehren, Ergebnis zeigen (erster Frame via `/thumbnail-frame`).
