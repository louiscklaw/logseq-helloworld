-
- ### Purpose:
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#purpose
	- To connect to the world while you’re working in linux environment at home…… inspired by [https://blog.wtako.net/view/23](https://blog.wtako.net/view/23)
	- [source link](https://blog.wtako.net/view/23)
-
- ### Requirements:
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#requirements
	- linux, gnome
	- python3, curl, gnome-mpv
-
- ### Install:
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#how-to-install
-
- ### Source:
  
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#source
  
  ```
  # RTHK31
  rthk31 () {
        link=$(curl -s -L https://www.rthk.hk/feeds/dtt/rthktv31_https.m3u8 | python2 -c 'import sys; list=sys.stdin.readlines();  print list[list.index("#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=2180000,RESOLUTION=1280x720,CODECS=\"avc1.66.30, mp4a.40.2\""\n")+1]')  && mpv $link &
  }
  
  # RTHK32
  rthk32 () {
        link=$(curl -s -L https://www.rthk.hk/feeds/dtt/rthktv31_https.m3u8 | python2 -c 'import sys; list=sys.stdin.readlines();  print list[list.index("#EXT-X-STREAM-INF:PROGRAM-ID=1,BANDWIDTH=2148000,RESOLUTION=1280x720,CODECS=\"avc1.66.30, mp4a.40.2\"\n")+1]')  && mpv $link &
  }
  ```
-
- ### to watch youtube under linux:
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#to-watch-youtube-under-linux
-
- to install
  
  ```
  pip3 install install youtube-dl mps-youtube==0.2.7
  ```
  
  to use
  
  ```
  mpsyt playurl https://www.youtube.com/watch?v=wcnBl6gNIhQ
  ```
-
- ### to watch ViuTV under linux:
  https://aboutme.louislabs.com/project-details/rthk31-rthk32-linux-viewer/#to-watch-viutv-under-linux
-
- command
	- ```bash
	  $ mpv http://viutv99-i.akamaihd.net/hls/live/265284/live1/stream4/streamPlaylist.m3u8
	  $ mpv http://viutv99-i.akamaihd.net/hls/live/265284/live1/master.m3u8
	  ```
-
- ### cable tv
- command
	- ```bash
	  $ mpv http://media.fantv.hk/m3u8/archive/channel2.m3u8
	  ```
- [12](https://aboutme.louislabs.com/project-list)
-