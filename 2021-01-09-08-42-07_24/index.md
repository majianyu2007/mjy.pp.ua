# 安装锐速有这么玄学么？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376171&amp;ptid=760305" target="_blank"><font color="#999999">kra 发表于 2020-10-30 17:29</font></a></font><br />
在不同商家的使用 ，试验。<br />
wget -N --no-check-certificate &quot;https://github.000060000.xyz/tcpx.sh&quot; &amp;&amp; c ...</blockquote></div><br />
ruvds家可以装上锐速，ovh 17.88刀 dd了debian9，装不了锐速

主要原因是萌咖大佬删库了，导致很多脚本直接废了

不行就装bbr呗&nbsp;&nbsp;bbr效果也可以的

用 centos 8.0 吧 自带的，命令一键激活<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376277&amp;ptid=760305" target="_blank"><font color="#999999">ufo629 发表于 2020-10-30 17:46</font></a></font><br />
用 centos 8.0 吧 自带的，命令一键激活</blockquote></div><br />
大佬，求命令

<i class="pstatus"> 本帖最后由 ufo629 于 2020-10-30 20:09 编辑 </i><br />
<br />
&nbsp; &nbsp; .

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376460&amp;ptid=760305" target="_blank"><font color="#999999">ufo629 发表于 2020-10-30 18:23</font></a></font><br />
BBR的执行下面三行命令自动执行。<br />
echo &quot;net.core.default_qdisc=fq&quot; &gt;&gt; /etc/sysctl.conf<br />
echo &quot;net.ipv ...</blockquote></div><br />
楼主要锐速，你发的是BBR！<br />
<br />
<img src="static/image/smiley/default/loveliness.gif" smilieid="28" border="0" alt="" />

挺多都这样的，不行就换bbr p 吧。。

<i class="pstatus"> 本帖最后由 蓝瘦香菇 于 2020-10-30 22:30 编辑 </i><br />
<br />
我几个机子都装上了，用的就是楼主第三条命令，真的玄<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> 

信则有^_^
