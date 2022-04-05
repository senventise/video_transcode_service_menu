# Video transcode service menu
Transcode video to HEVC in context menu.

## Requirements
[FFmpeg](https://ffmpeg.org/):
```
# transcode with GPU
ffmpeg -hwaccel cuda -i "$1" -c:v hevc_nvenc -c:a libopus -crf 26 "$1".opt.mp4"
```
[kdialog](https://github.com/KDE/kdialog): show dialogs

## Sceenshot
![context menu](https://raw.githubusercontent.com/senventise/video_transcode_service_menu/master/screenshot.png)
