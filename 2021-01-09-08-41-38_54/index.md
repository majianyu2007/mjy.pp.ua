# 跟virmach很熟的进来


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353428&amp;ptid=758532" target="_blank"><font color="#999999">wvps 发表于 2020-10-26 12:12</font></a></font><br />
换IP是可以的，但问题是换的IP是否还有验证问题。</blockquote></div><br />
照样被标记，按照IP端封的，好像还有198的没封

<i class="pstatus"> 本帖最后由 蓝瘦香菇 于 2020-10-26 13:54 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353854&amp;ptid=758532" target="_blank"><font color="#999999">maintell 发表于 2020-10-26 13:46</font></a></font><br />
试过了，不行</blockquote></div><br />
<br />
反正我可以，稳定一年了<img src="static/image/smiley/yct/007.gif" smilieid="46" border="0" alt="" /><br />
起初是为了解决没ipv6的问题<br />
你要服务器用ipv6访问谷歌避开验证<br />
ping google.com -c2 看看解析出来的是不是ipv6

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353898&amp;ptid=758532" target="_blank"><font color="#999999">蓝瘦香菇 发表于 2020-10-26 13:52</font></a></font><br />
反正我可以，稳定一年了</blockquote></div><br />
大佬，这种方法是可行的<br />
通过v2翻出去，在浏览器查看ip只能查看到ipv6的吧

我的是LA，两个IP一样要人机验证……

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353909&amp;ptid=758532" target="_blank"><font color="#999999">wvps 发表于 2020-10-26 13:54</font></a></font><br />
大佬，这种方法是可行的<br />
通过v2翻出去，在浏览器查看ip只能查看到ipv6的吧 ...</blockquote></div><br />
嗯，默认ipv6优先，可以在这个地方控制<br />
/etc/gai.conf<br />
往下找<br />
#&nbsp; &nbsp; For sites which prefer IPv4 connections change the last line to<br />
#<br />
#precedence ::ffff:0:0/96&nbsp;&nbsp;100<br />
<br />
需要ipv4优先就把上面这行#号去掉

同样要验证，很烦

几块钱一年的机器 还要满足你这么无耻的要求，没问题我们可以换，换一次50刀包过验证<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353407&amp;ptid=758532" target="_blank"><font color="#999999">wvps 发表于 2020-10-26 12:07</font></a></font><br />
是不是很烦？我想花钱换个干净的了</blockquote></div><br />
告诉你个曲线方法，用ipv6 通道进google

<div class="quote"><blockquote><font color="#999999">Geekman 发表于 2020-10-26 14:19</font><br />
<font color="#999999">告诉你个曲线方法，用ipv6 通道进google</font></blockquote></div><br />
求方法，被google这个问题困绕很久了

换IP 没得挑吧~<img id="aimg_VSlln" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
