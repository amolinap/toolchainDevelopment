# Comandos FFMPEG

## Homebrew

The Missing Package Manager for macOS (or Linux)

[Página principal](https://brew.sh/)

### Install Homebrew:

```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## FFMPEG

A complete, cross-platform solution to record, convert and stream audio and video.

[Página principal](https://ffmpeg.org/)

### Install FFmpeg:

```
brew install ffmpeg
```

### Comandos básicos:

**`ffmpeg -i video.m4v video.mp4`** Cambiar extensión de video

**`ffmpeg -i SPARTAAM_CENCASANT.mov -vf format=yuv420p SPARTAAM_CENCASANT.mp4`** Videos con vista miniatura

**`ffmpeg -i dia-01.mov -vf 'setpts=1/32*PTS' output3.mp4`** Velocidad 32x
**`ffmpeg -i el_video.avi -an sin_audio.avi`** Video sin audio

**`ffmpeg -start_number 439 -i IMG_8%03d.jpg -s 720x480 -b 3000k video.mp4`** Generar videos con imagenes

**`ffmpeg -i AeropuertoVeracruz.mpg -b 2000k AeropuertoVeracruz.mp4`** Comprimir video 8.64 GB a 1.62 GB

### Comandos avanzados:

**`ffmpeg -i input.mp4 -c copy -aspect 4/3 output.mp4`** Para quitar efecto ojo de pescado GoPro 16:9 a 4:3