---
name: short-aus-video
description: Erstellt aus einem Langvideo einen 9:16-Short: Abschnitt schneiden, auf 1080x1920 bringen, Untertitel einbrennen.
---

# Long -> Short (9:16)

Delegiere an `video-cutter`. Frag Start/Ende (oder nutze `/highlight-finder`).

## Pipeline
1. Schneiden: `ffmpeg -ss START -to ENDE -i in.mp4 -c:v libx264 -c:a aac clip.mp4`
2. Auf 9:16 (mittiger Crop): `ffmpeg -i clip.mp4 -vf "crop=ih*9/16:ih,scale=1080:1920" -c:a copy vert.mp4`
3. Untertitel: `/untertitel` -> `/untertitel-burn` auf vert.mp4.

Ergebnis: fertiger Short. Zielgruppe: spirituelle Frauen und Coaches. Ton: warm, kleines „du“, Resonanz statt Hype, KEINE Gedankenstriche. Marke, Stimme und Website kommen aus dem jeweiligen Auftrag.
