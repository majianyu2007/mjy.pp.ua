# 播放GD盘电影的脚本


播放GD盘电影：Emby索引路径转PotPlayer自动播放脚本<br />
<br />
https://youtu.be/fk4YLZOjUlE<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353996&amp;ptid=758588" target="_blank"><font color="#999999">BWH 发表于 2020-10-26 14:10</font></a></font><br />
所以，脚本呢</blockquote></div><br />
https://youtu.be/fk4YLZOjUlE<br />
<br />
播放GD盘电影：Emby索引路径转PotPlayer自动播放脚本<br />


好像可以试一下，正好搭了个emby挂GD盘<img id="aimg_xslVj" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

楼主可以在试试<br />
ffmpeg推流GD盘里面的视频播放么？<br />
我之前测试只能播放第一集，后面的就不会播放了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354523&amp;ptid=758588" target="_blank"><font color="#999999">funkys 发表于 2020-10-26 16:01</font></a></font><br />
楼主可以在试试<br />
ffmpeg推流GD盘里面的视频播放么？<br />
我之前测试只能播放第一集，后面的就不会播放了。 ...</blockquote></div><br />
virmach的 vps&nbsp;&nbsp;安装 emby，就是调用 ffmpeg 推流的，<br />
很占用CPU，只能看 720P，高码流的还会卡死。<br />
使用 nginx web方式播放，对vps负载很小 

收藏一下

脚本拿出来试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354493&amp;ptid=758588" target="_blank"><font color="#999999">sRGB 发表于 2020-10-26 15:56</font></a></font><br />
https://youtu.be/fk4YLZOjUlE<br />
<br />
播放GD盘电影：Emby索引路径转PotPlayer自动播放脚本</blockquote></div><br />
太麻烦了啊，直接webdav啊 rclone自带功能

直接rclone挂载啊大哥。。。

卧槽，这个思路太骚了，牛逼牛逼。<br />
<br />
配合cf的网盘直链程序，可以继续玩出花啊<br />
emby网页里显示的地址转换成网盘的直链，判断一下浏览器ua，调用potplayer（电脑）或者nplayer（手机）<br />
国内直接走cf，再用host文件自选一个速度快的ip，嘿嘿嘿<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
<br />
8楼那个油猴脚本还可以直接在emby里加一个按钮<br />
<br />
想法有了就差一个程序员了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
<br />
我只会AHK，等一个大佬织毛衣
