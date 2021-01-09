# 【反馈】EHEH首次手动执行后不再运行，


刚把大部分小鸡都安装上EHEH，但遇到过问题，首次手动执行之后就不上传数据了，查看了安装脚本一步一步排查终于发现问题。<br />
<br />
root用户安装，会新建一个EHEH用户来执行cron<br />
<br />
安装完，如果是dabian和ubuntu会提示<br />
|&nbsp; &nbsp;Debian/ubuntu的默认shell已经切换成了dash。如需马上推送一次数据，请手动执行以下命令<br />
|&nbsp; &nbsp;/etc/EHEH/eheh-agent.sh &amp;&amp; chown -Rf EHEH.EHEH /etc/EHEH/ <br />
<br />
实测执行完，有两个log文件是root用户组的，导致后面EHEH写不了数据，再次执行chown -Rf EHEH.EHEH /etc/EHEH/ 才正常。<br />
<br /><div class="blockcode"><div id="code_HB4"><ol><li>root@instance-1:~# cd /etc/EHEH/<br /><li>root@instance-1:/etc/EHEH# ll<br /><li>-bash: ll: command not found<br /><li>root@instance-1:/etc/EHEH# ls -l<br /><li>total 24<br /><li>-rw-r--r-- 1 root root&nbsp; &nbsp;&nbsp;&nbsp;7 Oct 25 13:22 eheh-agent.log<br /><li>-rwx------ 1 EHEH EHEH 10297 Oct 25 12:57 eheh-agent.sh<br /><li>-rwx------ 1 EHEH EHEH&nbsp; &nbsp; 33 Oct 25 12:57 eheh-auth.log<br /><li>-rw-r--r-- 1 EHEH EHEH&nbsp; &nbsp;&nbsp;&nbsp;0 Oct 25 13:21 eheh-cron.log<br /><li>-rw-r--r-- 1 root root&nbsp; &nbsp; 70 Oct 25 13:21 eheh-data.log</ol></div><em onclick="copycode($('code_HB4'));">复制代码</em></div><br />
<br />
另外提个建议，能不能界面做小一点，让屏幕一次显示更多小鸡<br />
还有就是分享是不是一个地址只能显示一台小鸡？能不能像uptimebot那样弄一个不用登录显示所有小鸡的页面<br />
<br />
一堆垃圾小鸡<br />
<img id="aimg_YiX45" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://p.pstatp.com/origin/13751000163230df3dcc8" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

反馈收到，感谢支持！&nbsp;&nbsp;请问下安装完有手动执行/etc/EHEH/eheh-agent.sh &amp;&amp; chown -Rf EHEH.EHEH /etc/EHEH/这个命令吗？如果有，的确是问题，稍后处理下。界面的想法我后续优化下，没专业前端，纯靠我这个后端，不足地方多担待。分享功能已经在路上了，敬请期待

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350060&amp;ptid=758271" target="_blank"><font color="#999999">Eric.c 发表于 2020-10-25 15:32</font></a></font><br />
反馈收到，感谢支持！&nbsp;&nbsp;请问下安装完有手动执行/etc/EHEH/eheh-agent.sh &amp;&amp; chown -Rf EHEH.EHEH /etc/EHEH ...</blockquote></div><br />
对的，安装完手动执行/etc/EHEH/eheh-agent.sh &amp;&amp; chown -Rf EHEH.EHEH 面板只有第一次数据，之后就失联了<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350117&amp;ptid=758271" target="_blank"><font color="#999999">hjvn2211445 发表于 2020-10-25 15:43</font></a></font><br />
对的，安装完手动执行/etc/EHEH/eheh-agent.sh &amp;&amp; chown -Rf EHEH.EHEH 面板只有第一次数据，之后就失联 ...</blockquote></div><br />
好，那是&amp;&amp;后没执行的感觉。我调试一下

感谢！<br />
<br />
所反馈bug，已做了处理。后半句无效执行应该是脚本执行中出现了些问题。目前最快处理方法是提示用户输入2次命令。<br />
<br />
因为很多debian默认不安装netstat，导致命令出错，尔后命令无法执行。

<i class="pstatus"> 本帖最后由 nilvae 于 2020-10-26 09:23 编辑 </i><br />
<br />
每次添加一个节点 需要自己手动刷新 能否在添加执行命令界面下方设置个 添加完成刷新的按钮，或者在添加节点按钮旁边添加一个刷新按钮

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9352445&amp;ptid=758271" target="_blank"><font color="#999999">nilvae 发表于 2020-10-26 09:21</font></a></font><br />
每次添加一个节点 需要自己手动刷新 能否在添加执行命令界面下方设置个 添加完成刷新的按钮，或者在添加节 ...</blockquote></div><br />
你去加多一台看看：） 

ok了 这次自动出来了

另外提个建议，能不能界面做小一点，让屏幕一次显示更多小鸡<br />
-------------<br />
1.当服务器超过10台的时候，行高自动缩短一半以上，<br />
2.默认显示50台服务器每页。

全球工单论坛<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img id="aimg_OW4LD" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
