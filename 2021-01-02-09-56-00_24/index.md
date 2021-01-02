# PLEX反代加速求教


2O装了个plex，但是到国内速度太慢了，视频不太流畅。入了个olink想反代加速。<br />
我是这么做的，在olink上建个站反代2O的ip:32400，然后在plex设置Custom server access URLs。<br />
但是弄好后看视频好像流量并没有走olink，还需要怎么做啊

你直接olink转发个端口呗

plex关闭外网访问，服务器里装个nginx反带一下plex，&nbsp;&nbsp;再用olink反带nginx

<i class="pstatus"> 本帖最后由 鼎剑阁 于 2020-11-4 19:55 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403256&amp;ptid=762469" target="_blank"><font color="#999999">streamer 发表于 2020-11-4 19:46</font></a></font><br />
plex关闭外网访问，服务器里装个nginx反带一下plex，&nbsp;&nbsp;再用olink反带nginx</blockquote></div><br />
<br />
现在plex服务器建个站反代到127.0.0.1：32400，然后再在olink反代到plex这个站吗？<br />
关闭外网访问以后如果再想打开的话又该怎么做呢，还能通过域名或者ip：32400访问吗<img id="aimg_Xlgl3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403276&amp;ptid=762469" target="_blank"><font color="#999999">鼎剑阁 发表于 2020-11-4 19:54</font></a></font><br />
现在plex服务器建个站反代到127.0.0.1：32400，然后再在olink反代到plex这个站吗？<br />
关闭外网访问以后如果 ...</blockquote></div><br />
参考这个https://yangmaopubu.com/187.html<br />
<br />
反代后就可以访问了啊，打开外网流量就不走反代的了 直接走IP:32400了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403696&amp;ptid=762469" target="_blank"><font color="#999999">streamer 发表于 2020-11-4 21:34</font></a></font><br />
参考这个https://yangmaopubu.com/187.html<br />
<br />
反代后就可以访问了啊，打开外网流量就不走反代的了 直接走I ...</blockquote></div><br />
主要是我不知道只反代ip行不行，需不需要plex绑定域名

frp直接反代内网端口 直接打洞比转发好
