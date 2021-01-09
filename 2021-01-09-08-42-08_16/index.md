# 安装探针出错，求助


Last-modified header missing -- time-stamps turned off.<br />
2020-10-30 14:21:16 (49.0 MB/s) - ‘caddy_install.sh’ saved [5601/5601]<br />
<br />
--2020-10-30 14:21:16--&nbsp;&nbsp;https://caddyserver.com/download/linux/amd64?license=personal<br />
Resolving caddyserver.com (caddyserver.com)... 165.227.20.207, 2604:a880:2:d0::21b0:6001<br />
Connecting to caddyserver.com (caddyserver.com)|165.227.20.207|:443... connected.<br />
HTTP request sent, awaiting response... 404 Not Found<br />
2020-10-30 14:21:16 ERROR 404: Not Found.<br />
<br />
<br />
gzip: stdin: unexpected end of file<br />
tar: Child returned status 1<br />
tar: Error is not recoverable: exiting now<br />
[错误] Caddy 解压失败或压缩文件错误 !<br />
[错误] Caddy安装失败，请手动部署，Web网页文件位置：<br />
<br />
<br />
<br />
小白求助怎么解决？

https://github.com/CokeMine/ServerStatus-Hotaru

404 Not Found，可能是以前caddy1时期的脚本。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375120&amp;ptid=760232" target="_blank"><font color="#999999">江户川柯南 发表于 2020-10-30 14:29</font></a></font><br />
https://github.com/CokeMine/ServerStatus-Hotaru</blockquote></div><br />
这个试了也一样的呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375128&amp;ptid=760232" target="_blank"><font color="#999999">Fei 发表于 2020-10-30 14:29</font></a></font><br />
404 Not Found，可能是以前caddy1时期的脚本。</blockquote></div><br />
要怎么解决呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375158&amp;ptid=760232" target="_blank"><font color="#999999">oppoter 发表于 2020-10-30 14:35</font></a></font><br />
要怎么解决呢</blockquote></div><br />
<br />
自己改caddy下载地址，或换成caddy2。<br />
https://github.com/caddyserver/caddy/releases/tag/v1.0.4

fuck caddy，github有已经改了的

https://www.sbblog.cn/archives/19.html

自己手动caddy

https://idcfq.com/archives/63.html<br />
我一直用这个。没出错过
