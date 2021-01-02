# 哪个dns 解析服务可以强制走https？


楼主你在搞笑吗，cloudflare也是80跳转443.我猜你是开了cloudflare的cdn,别急，443端口有流量早晚也是封

301的意思吗&nbsp; &nbsp; 源站或者cdn设置就行<img id="aimg_bDbl6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

楼主根本没有搞明白cdn dns http https的区别...<br />
dns只能返回ip不能返回端口<br />
http访问cf 的cdn 会301到https端口 而不是“dns设置了443端口” dns协议决定了他只能返回ip地址<img id="aimg_R3VUv" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 pengxp1996 于 2020-11-4 22:52 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403200&amp;ptid=762466" target="_blank"><font color="#999999">keramist 发表于 2020-11-4 19:32</font></a></font><br />
有毛用 <br />
必须在dns端就变为https<br />
否则访问未北岸80端口 不会跳转https </blockquote></div><br />
<br />
DNS并不具备这样的功能，你这个要求，DNS只能说：做不到<br />
<br />
但是你这个想法很不错，利用cf进行一次跳转
