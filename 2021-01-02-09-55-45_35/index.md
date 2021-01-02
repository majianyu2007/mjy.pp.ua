# 卧槽良心轻量被植入挖矿后门


不知道怎么时候被植入了挖矿病毒，我了个去<br />
<br />
表现就是流量一直跑，CPU很高<br />
<br />
然后删掉了整个文件夹，观察一段时间<br />
<br /><div class="blockcode"><div id="code_qDt"><ol><li>[root@VM-0-12-centos ~]# ps -ef |grep tsm<br /><li>root&nbsp; &nbsp;&nbsp;&nbsp;13851 32292&nbsp;&nbsp;0 22:47 ?&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;00:00:00 timeout 3h ./tsm -t 515 -f 1 -s 12 -S 10 -p 0 -d 1 p ip<br /><li>root&nbsp; &nbsp;&nbsp;&nbsp;13853 13851&nbsp;&nbsp;0 22:47 ?&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;00:00:00 /bin/bash ./tsm -t 515 -f 1 -s 12 -S 10 -p 0 -d 1 p ip<br /><li>root&nbsp; &nbsp;&nbsp;&nbsp;13859 13853&nbsp;&nbsp;0 22:47 ?&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;00:00:00 /tmp/.X25-unix/.rsync/c/lib/64/tsm --library-path /tmp/.X25-unix/.rsync/c/lib/64/ /tmp/.X25-unix/.rsync/c/tsm64 -t 515 -f 1 -s 12 -S 10 -p 0 -d 1 p ip</ol></div><em onclick="copycode($('code_qDt'));">复制代码</em></div>

帮顶，被扫了？<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351756&amp;ptid=758407" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-25 23:01</font></a></font><br />
帮顶，被扫了？</blockquote></div><br />
不知道，我还换了端口的，后面有空再调查

跑了多少流量<img id="aimg_PNNtc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351780&amp;ptid=758407" target="_blank"><font color="#999999">wolfling45 发表于 2020-10-25 23:05</font></a></font><br />
跑了多少流量</blockquote></div><br />
每天20个G左右吧

能及时发现还不错了，不懂技术的不知道有多少

搜了一下X25-unix，感染这个木马得挺多得<img id="aimg_E4Pnk" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351799&amp;ptid=758407" target="_blank"><font color="#999999">微笑着吃饭 发表于 2020-10-25 23:09</font></a></font><br />
能及时发现还不错了，不懂技术的不知道有多少</blockquote></div><br />
最近一两周才开始跑的，刚开始还没在意

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351801&amp;ptid=758407" target="_blank"><font color="#999999">wolfling45 发表于 2020-10-25 23:10</font></a></font><br />
搜了一下X25-unix，感染这个木马得挺多得</blockquote></div><br />
大家都注意一下

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351811&amp;ptid=758407" target="_blank"><font color="#999999">scuboy2008 发表于 2020-10-25 23:12</font></a></font><br />
大家都注意一下</blockquote></div><br />
多谢大佬提醒，小白面对这个还真没办法
