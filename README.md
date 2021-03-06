# Installation
```bash
pip install Ydl
```
Jupyter or Colab
```bash
!pip install Ydl
```
# Pypi
[Ydl](https://pypi.org/project/Ydl/)
# Usage

```python
import ydl

YouTube_url = "https://www.youtube.com/watch?v=xxxxxx"

itag = 22

path = '/video/foo' #Excluding the extension

y = ydl.YouTube_Download(YouTube_url)
print(y.downloadable()) #['249 - audio only (tiny)(webm)', '250 - audio only (tiny)(webm)', '251 - audio only (tiny)(webm)', '140 - audio only (tiny)(m4a)', '160 -256x144 (144p)(mp4)', '278 - 256x144 (144p)(webm)', '394 - 256x144 (144p)(mp4)', '133 - 426x240 (240p)(mp4)', '395 - 426x240 (240p)(mp4)','242 - 426x240 (240p)(webm)', '134 - 640x360 (360p)(mp4)', '243 - 640x360 (360p)(webm)', '396 - 640x360 (360p)(mp4)', '135 - 854x480 (480p)(mp4)', '244 - 854x480 (480p)(webm)', '397 - 854x480 (480p)(mp4)', '136 - 1280x720 (720p)(mp4)', '398 - 1280x720 (720p)(mp4)', '247 - 1280x720 (720p)(webm)', '399 - 1920x1080 (1080p)(mp4)', '137 - 1920x1080 (1080p)(mp4)', '248 - 1920x1080 (1080p)(webm)', '18 - 640x360 (360p)(mp4)', '22 - 1280x720 (720p)(mp4)']

print(y.entities) #{'title': '(title)', 'uploader': '(uploader)', 'upload_date': '(data)', 'view_count': (view_count), 'thumbnail': '(thumbnail_url)'}

print(y.get_url(itag)) #https://xxxxxx.googlevideo.com/videoplayback?xxxxxx

y.ydl(itag, path) #Download at '/video/test.(ext)'

print(y.get_ext(itag) #mp4
```


# Acknowledgments
[youtube-dl](https://github.com/ytdl-org/youtube-dl)
# License

ydl is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).
