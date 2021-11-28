---
layout: post
title: How To Extract Audio From YouTube Videos
---

When I record [freestyles](https://dylanhand.com/2020/11/12/word-generator-freestyle/), my normal process is to open YouTube, find beats, and then download them one-by-one using one of the various ad-ridden and janky sites you might find with some Googling. Turns out there's a better way.

[yt-dlp](https://youtube-dl.org/) lets you extract audio from a YouTube video right from the command line. You can also just download the full video if you want.

On a Mac, install it with:

```
$ brew install yt-dlp/taps/yt-dlp
```

Then get the audio of a video with:

```
$ yt-dlp -x --audio-format mp3 https://youtu.be/us5CDWzIet4
```

You can also do it for multiple videos at a time:

```
$ yt-dlp -x --audio-format mp3 https://youtu.be/us5CDWzIet4 https://youtu.be/8SAnu1hd04U 
```

Stoked. This is a much faster and cleaner way to download audio from YouTube.