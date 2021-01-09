# 谁会搞pt上传到googledrive


学习大佬们的答案！<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

搜googledrive的时候偶然看见这篇，我来给个简单点的方案<br />
flexget传入＋qbittorrent+rclone，需求大盘鸡<br />
小白可用这个项目一键，作者也正在坛里混，尽量用纯净系统：https://github.com/amefs/quickbox-lite<br />
flexget自己研究下，网上有很多小白教程，能正常用就行，这个脚本安装的qb的传入端口是15191<br />
qb设置改一下第一页的,把没下载完成的和已完成下载的设置成不同目录<br />
rclone设置好自己的gd盘，然后设个定时任务隔段时间运行rclone copy命令把已完成下载的目录复制到gd里就完事了

先马克一下，学习

qb rclone 我发过

pt不好弄啊，考核的话下载完成的文件都不能删。<br />
<br />
之前想用gcp，后来放弃了。<br />
<br />
直接mount下载速度很受影响，而且不确定能不能考核<img id="aimg_ZM7K3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
