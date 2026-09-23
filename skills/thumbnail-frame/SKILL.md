---
name: thumbnail-frame
description: Extrahiert mit ffmpeg einen Einzelframe aus einem Video als Thumbnail-Bild.
---

# Thumbnail-Frame

## Befehl
`ffmpeg -ss ZEIT -i in.mp4 -frames:v 1 -q:v 2 thumb.png`

Zeit z.B. `00:00:07`. Danach Frame anzeigen und ggf. als Thumbnail-Basis fuer `/yt-thumbnail` nutzen.
