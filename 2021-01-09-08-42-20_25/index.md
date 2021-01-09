# Centos 如何关闭 journal


用命令也限制不了,老是会生成,请问如何关闭 journal 生成的LOG文件,...<br />
<br />
话说 <br />
<br />
/run/log/journal/2d974dsc4155sw111424 <br />
<br />
可以直接删除吗

log太大定时删除就好了，journalctl --vacuum-time=1d

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9383615&amp;ptid=760826" target="_blank"><font color="#999999">Bill_Carson 发表于 2020-11-1 06:14</font></a></font><br />
log太大定时删除就好了，journalctl --vacuum-time=1d</blockquote></div><br />
这个命令 打了 ,硬盘空间还是不会自动缩小 需要重启服务器才会显示硬盘空间空了出来,蛋疼

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9383616&amp;ptid=760826" target="_blank"><font color="#999999">linode-jspinosi 发表于 2020-11-1 06:16</font></a></font><br />
这个命令 打了 ,硬盘空间还是不会自动缩小 需要重启服务器才会显示硬盘空间空了出来,蛋疼 ...</blockquote></div><br />
磁盘未释放是因为进程没有退出，可以看看https://mp.weixin.qq.com/s/RyBjrjK378-yAUFAUcr-2A

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9383623&amp;ptid=760826" target="_blank"><font color="#999999">Bill_Carson 发表于 2020-11-1 06:34</font></a></font><br />
磁盘未释放是因为进程没有退出，可以看看https://mp.weixin.qq.com/s/RyBjrjK378-yAUFAUcr-2A ...</blockquote></div><br />
我能不能用宝塔直接关闭这个进程

systemctl stop systemd-journal
