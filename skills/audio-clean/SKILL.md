---
name: audio-clean
description: Saeubert Video-Audio mit ffmpeg: Lautheit normalisieren und lange Stillen kuerzen.
---

# Audio saeubern

## Befehle
- Lautheit normalisieren: `ffmpeg -i in.mp4 -af loudnorm=I=-16:TP=-1.5:LRA=11 -c:v copy out.mp4`
- Stille kuerzen: `ffmpeg -i in.mp4 -af silenceremove=stop_periods=-1:stop_duration=0.6:stop_threshold=-35dB -c:v copy out.mp4`

Delegiere an `video-cutter`, real ausfuehren.
