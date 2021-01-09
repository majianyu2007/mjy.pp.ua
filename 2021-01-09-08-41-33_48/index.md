# 为什么输入脚本执行没反应呢


<font size="5">很奇怪 执行脚本没反应， DD的debian9系统全是问题，绿云独有，别家DD后都正常，不知道缺少啥组件，也不报错 日了鬼</font><br />
<br />
<img id="aimg_rqNJn" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/27/CkmX4NcnpWUDftg.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 hjvn2211445 于 2020-10-27 09:34 编辑 </i><br />
<br />
将脚本下载下来，再执行，<br />
wget git.io/superspeed &amp;&amp;bash&nbsp;&nbsp;superspeed<br />
<br />
再不显示就bash -x&nbsp;&nbsp;superspeed

说明卡在了curl上

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9357493&amp;ptid=758842" target="_blank"><font color="#999999">hjvn2211445 发表于 2020-10-27 09:32</font></a></font><br />
将脚本下载下来，再执行，<br />
wget git.io/superspeed &amp;&amp;bash&nbsp;&nbsp;superspeed</blockquote></div><br />
好像系统有毛病<img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" /><br />
<br />
root@debian:~#<br />
root@debian:~# wget git.io/superspeed &amp;&amp;bash&nbsp;&nbsp;superspeed<br />
--2020-10-26 22:05:23--&nbsp;&nbsp;http://git.io/superspeed<br />
Resolving git.io (git.io)... 35.153.20.238, 54.84.72.55, 52.203.100.2, ...<br />
Connecting to git.io (git.io)|35.153.20.238|:80...
