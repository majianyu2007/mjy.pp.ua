# 腾讯云服务器安装BBR Plus 过程中失联


<i class="pstatus"> 本帖最后由 dmking923 于 2020-10-30 17:34 编辑 </i><br />
<br />
<font size="4"><br />
国内服务器，centos7.6系统<br />
<br />
安装bbr plus过程中，执行完第一步安装后失联，半个多小时联不上。<br />
<br />
只能是重置系统，又才连上...<br />
<br />
有没有同经历的大佬，指点下，该怎么安装？<br />
<br />
用的是一键脚本：wget --no-check-certificate -O tcp.sh https://github.com/cx9208/Linux-NetSpeed/raw/master/tcp.sh &amp;&amp; chmod +x tcp.sh &amp;&amp; ./tcp.sh</font>

看脚本就有装内核，还叫没动内核？这样证明这内核不适合这机器用，自己找个合适的差不多的内核装了，再看脚本执行得了<br />


是不是动内核了

装了会不会 减速？<br />


<i class="pstatus"> 本帖最后由 dmking923 于 2020-10-30 17:41 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376209&amp;ptid=760317" target="_blank"><font color="#999999">KuYeHQ 发表于 2020-10-30 17:34</font></a></font><br />
是不是动内核了</blockquote></div><br />
<br />
应该没有...正常来说，会有选择卸载或是不卸载内核（如果出来了肯定会选不卸载），但是这块直接没有出来选项，直接到完成重启。重启后就连不上了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376212&amp;ptid=760317" target="_blank"><font color="#999999">vzker 发表于 2020-10-30 17:34</font></a></font><br />
装了会不会 减速？</blockquote></div><br />
<br />
这个就真不知道了，装这个就是心里安慰，自WEI的过程。<img src="static/image/smiley/coolmonkey/03.gif" smilieid="58" border="0" alt="" />

国内服务器，也没多大必要加速，不必折腾

你用 centos 8.0的里面有自带BBR。

装了好像没有什么效果，感觉

c手动开启BBR就行。国内还用plus干啥。反正就一个心理暗示作用。
