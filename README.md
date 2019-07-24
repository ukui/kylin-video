kylin-video
===========

Kylin Video utilizes MPV and MPlayer as background play engine (use MPV by default). Its GUI front end is written by Qt5. Plus, it supports both x86 and ARM platform. As a powerful video player, Kylin Video supports most of the audio and video formats. Functions of shortcut keys/ preview/ screenshot/ sound settings/ subtitles and so on are provided. Users can even customize settings as they like.

![image](./doc/appearence.png)

Installation
============

qmake

make

sudo make install


How to report bugs
==================

Bugs should be report to the kylin-video bug tracking system:
    https://github.com/ukui/kylin-video/issues


Snap
==================

snapcraft

snapcraft clean

sudo snap install kylin-video_1.1.6_amd64.snap --devmode

sudo snap install kylin-video_1.1.6_amd64.snap --classic --dangerous

sudo snap install kylin-video_1.1.6_amd64.snap --stable --dangerous

sudo snap remove kylin-video

unsquashfs -l kylin-video_1.1.6_amd64.snap | less

unsquashfs kylin-video_1.1.6_amd64.snap

查看已经存在的plug及slot:   snap interfaces (snapcraft plugins    snapcraft list-plugins)

处在snapcraft中最核心的是parts。parts是一些软件或数据被用来构造snap包的，或是用来编译其它软件的，每个part是由一个plugin来管理的，并且通常是互相独立的。


Git
==================

分支1.1.6

新建分支：git branch 1.1.6

切换分支：git checkout 1.1.6

上传分支：git push origin 1.1.6


ts2po
==================

sudo apt install translate-toolkit

ts2po -i kylin-video_fr.ts -o kylin-video.pot

po2ts -i kylin-video_fr.po kylin-video_fr.ts


TODO
==================

+ playlist: load_m3u load_pls  loadXSPF 
