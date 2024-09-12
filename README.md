# down_to_m3u8_video
简单示例，使用多线程下载m3u8媒体文件

Install requirements.
```
pip3 install -r requirements.txt
```

url.txt 只能是单个URL链接，程序没做多个m3u8循环任务
```
http://192.168.3.101/video/video.m3u8
```
```
cat video.m3u8
```
```
#EXTM3U
#EXT-X-VERSION:3
#EXT-X-TARGETDURATION:4
#EXT-X-MEDIA-SEQUENCE:0
#EXT-X-PLAYLIST-TYPE:VOD
#EXTINF:4.004000,
video0.jpeg
#EXTINF:4.004011,
video1.jpeg
#EXTINF:4.004000,
video2.jpeg
#EXTINF:4.004000,
video3.jpeg
#EXTINF:4.004011,
video4.jpeg
#EXTINF:4.004000,
video5.jpeg
```
Running demo.
```
python3 down_to_m3u8_video.py
```
---
下载完成后，在程序执行目录有个videos，存储下载好的媒体文件


