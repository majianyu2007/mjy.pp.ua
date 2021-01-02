# 求一个宝塔数据库自动重启脚本。。。


<font face="微软雅黑"><font size="5">wp数据库总是炸，不能时时刻刻守着。。。网上搜的自动重启脚本，挂上没作用，不知道是不是失效了，求一个最新版，谢谢</font></font>

删库塔还敢用？<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

帮顶，等技术大佬吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

宝塔 这毛病还没改啊 我现在都装5.5了 装了一个小皮 感觉1h1g比宝塔好点

勇士啊，不怕删库吗

自己百度宝塔数据库自动重启脚本

pgrep -x mysqld &amp;&gt; /dev/null<br />
if [ $? -ne 0 ];then<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;bash /www/server/panel/script/rememory.sh<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;/etc/init.d/mysqld start<br />
fi<img id="aimg_Mbp9L" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350268&amp;ptid=758266" target="_blank"><font color="#999999">majianyu 发表于 2020-10-25 16:19</font></a></font><br />
pgrep -x mysqld &amp;&gt; /dev/null<br />
if [ $? -ne 0 ];then<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;bash /www/server/panel/script/rememory.sh</blockquote></div><br />
网上流传的都是这个版本，，，，但是感觉没得用处啊啊

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350321&amp;ptid=758266" target="_blank"><font color="#999999">hdwan.net 发表于 2020-10-25 16:34</font></a></font><br />
网上流传的都是这个版本，，，，但是感觉没得用处啊啊</blockquote></div><br />
个人感觉1H1G还是有用的。<img id="aimg_m4MLt" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

通过shell命令不行吗
