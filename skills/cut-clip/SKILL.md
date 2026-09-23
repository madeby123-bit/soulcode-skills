---
name: cut-clip
description: Schneidet mit ffmpeg einen Abschnitt aus einem Video (Start/Ende), verlustfrei oder neu kodiert.
---

# Video schneiden (ffmpeg)

Delegiere an `video-cutter`. Frag nach Dateipfad, Start, Ende.

## Befehle
- Schnell/verlustfrei: `ffmpeg -ss START -to ENDE -i in.mp4 -c copy out.mp4`
- Framegenau (neu kodiert): `ffmpeg -i in.mp4 -ss START -to ENDE -c:v libx264 -c:a aac out.mp4`

Fuehre den Befehl real aus und melde die Ausgabedatei.
