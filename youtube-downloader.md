# yt-dlp
The repository: https://github.com/yt-dlp/yt-dlp

### Installation
``` bash
brew install yt-dlp
```

### How to Use
- Downloading chapters of a youtube video as separated video files
  ``` bash
   yt-dlp --split-chapters  [OPTIONS] [URL]
   ```
- Download all video in a playlist
  ``` bash
  yt-dlp --verbose -ci --download-archive "archive.txt" [YOUTUBE_URL_PLAY_LIST]
  ```

- Check available format for the video want to download
  ``` bash
  yt-dlp -F [URL_VIDEO_OR_PLAYLIST]
  ```
  Then we can download with available format id/code

  ``` bash
  yt-dlp -f 22 [URL_VIDEO_OR_PLAYLIST]
  ```

# Reference
1. https://superuser.com/questions/1567253/how-to-download-chapters-of-a-youtube-video-as-separate-video-files
2. https://write.corbpie.com/downloading-youtube-videos-and-playlists-with-yt-dlp/