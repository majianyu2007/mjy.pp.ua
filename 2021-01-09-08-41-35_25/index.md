# 播放GD盘电影的脚本


<i class="pstatus"> 本帖最后由 sRGB 于 2020-10-27 13:03 编辑 </i><br />
<br />
<img id="aimg_ls8qS" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/26/BjyeMlF7a6PHdg1.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
docker run -d -p 80:80 --name&nbsp;&nbsp;nginx-web --cpus 0.6&nbsp;&nbsp;--restart=always \<br />
&nbsp;&nbsp;-v /mnt/EmbyMedia:/usr/share/nginx/html/xxxxxx使用目录名当密码xxxxxx \<br />
&nbsp;&nbsp;-v /var/www:/usr/share/nginx/html&nbsp; &nbsp;nginx <br />
<br />
<br />
开始是使用 Virmach黑五机挂载 GD网盘 Emby 做索引。<br />
然后 VPS 软件编码解码能力太吃 CPU，容易滥用。<br />
所以想到了 PotPlayer 64 bit 播放 URL 视频原文件<br />
<br />
===================================<br />
vps 上开了 http，挂载了GD盘，然后这个 80端口只能 127.0.0.1访问，转接到 kcp上，<br />
<br />
本地vbox安装 虚拟机 debian 10,&nbsp;&nbsp;IP 192.168.1.111.&nbsp;&nbsp;,通过 kcp 转接到 80端口上。<br />
本地 也安装了 emby，使用vps的数据，来加速使用索引数据。 当然也可以转接<br />
<br />
======================================<br />
播放的时候 手工要 把&nbsp;&nbsp;EmbyMedia 路径 到URL 给PotPlayer播放视频<br />
emby_path = &quot;/mnt/EmbyMedia/&quot;<br />
http_url = &quot;http://192.168.1.111/&quot;<br />
然后想到了脚本，方便给自己看动漫，所以添加了自动调用播放器<br />
<br />
<img id="aimg_RXD9I" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="558" height="733" src="https://i.loli.net/2020/10/26/SFLW6VAIpKqz5n4.jpg" border="0" alt="" /><br />
<br />
脚本源码和使用视频链接地址<br />
<br />
https://youtu.be/fk4YLZOjUlE<br />
<br />
<br />
<img id="aimg_qZGup" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/27/oenH7wx5Z4Uuyks.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

支持技术<br />
现在白女票的一批GD都有翻车风险<br />
我的翻了一辆<br />
不敢用了

<img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" />不会用

Google drive播放次数太多的话会把对应的文件屏蔽掉，自用还可以，商用算了

所以，脚本呢

有点意思

啥？pyjio本？正经人电脑不装py<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
还是用cfworker方便

https://greasyfork.org/zh-CN/scripts/406811-embylaunchpotplayer

PY本地播放？没有网络版么？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9354151&amp;ptid=758588" target="_blank"><font color="#999999">aipage 发表于 2020-10-26 14:46</font></a></font><br />
PY本地播放？没有网络版么？</blockquote></div><br />
emby 有下载视频功能，可以播放哪个网址，但是你 pot播放器要开代理
