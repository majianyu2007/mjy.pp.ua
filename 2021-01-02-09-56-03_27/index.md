# 请教大家一个旁路由设置的问题


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404225&amp;ptid=762552" target="_blank"><font color="#999999">花样撸管冠军 发表于 2020-11-4 23:21</font></a></font><br />
简单看了一下问题，应该是主路由跟N1不同网段</blockquote></div><br />
好像是的,我看别人的教程,人家的主路由都是192.168开头的,我的是101.76开头的教育网ip

<i class="pstatus"> 本帖最后由 花样撸管冠军 于 2020-11-4 23:27 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404242&amp;ptid=762552" target="_blank"><font color="#999999">fule 发表于 2020-11-4 23:24</font></a></font><br />
好像是的,我看别人的教程,人家的主路由都是192.168开头的,我的是101.76开头的教育网ip ...</blockquote></div><br />
<br />
<img id="aimg_r6jtJ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/04/2I9qHgevOSZ1C4c.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_LUwR3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/04/UDjIcGbaq19k5d8.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404242&amp;ptid=762552" target="_blank"><font color="#999999">fule 发表于 2020-11-4 23:24</font></a></font><br />
好像是的,我看别人的教程,人家的主路由都是192.168开头的,我的是101.76开头的教育网ip ...</blockquote></div><br />
不是的，是你的设置的主路由ip跟N1不同网段，跟你拨号公网IP或者内网ip没关系，我截图了，你看下吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404272&amp;ptid=762552" target="_blank"><font color="#999999">花样撸管冠军 发表于 2020-11-4 23:29</font></a></font><br />
不是的，是你的设置的主路由ip跟N1不同网段，跟你拨号公网IP或者内网ip没关系，我截图了，你看下吧 ...</blockquote></div><br />
好的,谢谢老哥,我试一下

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404272&amp;ptid=762552" target="_blank"><font color="#999999">花样撸管冠军 发表于 2020-11-4 23:29</font></a></font><br />
不是的，是你的设置的主路由ip跟N1不同网段，跟你拨号公网IP或者内网ip没关系，我截图了，你看下吧 ...</blockquote></div><br />
大佬,我N1设置的是192.168.0.102,修改主路由ip是指修改主路由的wan口吗,还是主路由的LAN口,我的LAN口已经改成192.168.0.2了,但是WAN口那个ip是自动获取的,改成固定的话,192.168.0.1显示网段与LAN口IP地址冲突<br />
<br />


<div class="quote"><blockquote><font color="#999999">fule 发表于 2020-11-4 23:37</font><br />
<font color="#999999">大佬,我N1设置的是192.168.0.102,修改主路由ip是指修改主路由的wan口吗,还是主路由的LAN口,我的LAN口已经 ...</font></blockquote></div><br />
<img id="aimg_C80gJ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/04/tJI6URogV9XnxAk.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404333&amp;ptid=762552" target="_blank"><font color="#999999">花样撸管冠军 发表于 2020-11-4 23:48</font></a></font></blockquote></div><br />
大佬,我就是这样设置的,但还是进不去n1后台...显示超时,ping的时候显示无法访问目标主机

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404362&amp;ptid=762552" target="_blank"><font color="#999999">fule 发表于 2020-11-4 23:55</font></a></font><br />
大佬,我就是这样设置的,但还是进不去n1后台...显示超时,ping的时候显示无法访问目标主机 ...</blockquote></div><br />
N1网关设置成主路由了吗？

楼上正解，自动分配IP地址在主路由开，然后N1的网关设置成主路由的地址192.168.0.2<img id="aimg_g0d48" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

如果现在进不去N1的后台的话，把N1直连电脑，把电脑ip调成和N1同网段，然后再进N1后台设置网关为主路由，再插上试试<img id="aimg_AUkuD" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
