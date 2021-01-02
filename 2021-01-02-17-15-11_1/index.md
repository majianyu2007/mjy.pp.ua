# CloudFlare Worker能转发非标准端口吗


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9301026&amp;ptid=753719" target="_blank"><font color="#999999">dole 发表于 2020-10-14 19:51</font></a></font><br />
我是这样填的</blockquote></div><br />
https://pastebin.com/ijmb99SJ<br />
我这样是没问题的，你可以试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9301120&amp;ptid=753719" target="_blank"><font color="#999999">tkzc 发表于 2020-10-14 20:07</font></a></font><br />
https://pastebin.com/ijmb99SJ<br />
我这样是没问题的，你可以试试</blockquote></div><br />
感谢大佬 我去试试<img id="aimg_Ut5Sq" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

可以，域名后面加端口就行了

有端口限制的吧

<i class="pstatus"> 本帖最后由 大鸡鸡 于 2020-10-15 09:48 编辑 </i><br />
<br />
Cloudflare 支持的 HTTP 端口：<br />
80、8080、8880、2052、2082、2086、2095<br />
Cloudflare 支持的 HTTPS 端口：<br />
443、2053、2083、2087、2096、8443<br />
<br />
源站端口通过worker可以自己定义。<br />
<br />
例如：<br />
80-&gt;1234<br />
8080-&gt;12345<br />
8443-&gt;54321

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9302969&amp;ptid=753719" target="_blank"><font color="#999999">大鸡鸡 发表于 2020-10-15 09:47</font></a></font><br />
Cloudflare 支持的 HTTP 端口：<br />
80、8080、8880、2052、2082、2086、2095<br />
Cloudflare 支持的 HTTPS 端口：</blockquote></div><br />
具体在那里自定义

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9303110&amp;ptid=753719" target="_blank"><font color="#999999">cbbbb 发表于 2020-10-15 10:17</font></a></font><br />
具体在那里自定义</blockquote></div><br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />请我喝咖啡嘛

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9303118&amp;ptid=753719" target="_blank"><font color="#999999">大鸡鸡 发表于 2020-10-15 10:18</font></a></font><br />
请我喝咖啡嘛</blockquote></div><br />
求指点 大帅哥<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_dP5GG" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

没有明白……

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9302969&amp;ptid=753719" target="_blank"><font color="#999999">大鸡鸡 发表于 2020-10-15 09:47</font></a></font><br />
Cloudflare 支持的 HTTP 端口：<br />
80、8080、8880、2052、2082、2086、2095<br />
Cloudflare 支持的 HTTPS 端口：</blockquote></div><br />
<img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" />大佬 主要是worker过去提示ssl错误/无法ip访问<img id="aimg_lSzks" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
