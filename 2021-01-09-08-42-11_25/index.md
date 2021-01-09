# cera可算会装虚拟机能上网了，再请教下装系统默认分区问题


<i class="pstatus"> 本帖最后由 斌斌 于 2020-10-31 03:54 编辑 </i><br />
<br />
可算自己弄好了桥接能联网了，送机器和付费都没人帮忙，好惨，还是得靠自己研究。。看看下面这个问题有会的么。，<br />
下面这样安装完了分的100G硬盘，默认又给/home 里面分配了。应该不选择标准分区吧？不知道选哪个具体怎么设置。<br />
[root<a href="https://www.hostloc.com/home.php?mod=space&amp;uid=22998" target="_blank">@localhost</a> ~]# df -h<br />
Filesystem&nbsp; &nbsp;&nbsp; &nbsp;Size&nbsp;&nbsp;Used Avail Use% Mounted on<br />
devtmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;3.9G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;3.9G&nbsp; &nbsp;0% /dev<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;3.9G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;3.9G&nbsp; &nbsp;0% /dev/shm<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;3.9G&nbsp;&nbsp;8.5M&nbsp;&nbsp;3.9G&nbsp; &nbsp;1% /run<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;3.9G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;3.9G&nbsp; &nbsp;0% /sys/fs/cgroup<br />
/dev/vda3&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;50G&nbsp;&nbsp;2.1G&nbsp; &nbsp;48G&nbsp; &nbsp;5% /<br />
/dev/vda5&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;42G&nbsp; &nbsp;33M&nbsp; &nbsp;42G&nbsp; &nbsp;1% /home<br />
/dev/vda1&nbsp; &nbsp;&nbsp; &nbsp;1014M&nbsp;&nbsp;141M&nbsp;&nbsp;874M&nbsp;&nbsp;14% /boot<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;783M&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;783M&nbsp; &nbsp;0% /run/user/0<br />
<br />
<br />
下面四个步骤<br />
<br />
一<br />
<img id="aimg_S0oHJ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/31/BNqnw8.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
二<br />
<img id="aimg_yGxWW" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/31/BNquTS.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
三<br />
<img id="aimg_ibBgw" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/31/BNqmef.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
四<br />
<img id="aimg_IJK8V" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/31/BNqZOP.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

斌斌 你好 我觉得你新买的服务器很棒

你问的我不会，依然前排等鸡

你是想删掉数据盘 全部分给/ ？

看红帽官方文档，自动分区不超过50G，不会分给/home，反之就会像你那样

这个真不会，帮你顶上去，让会的大佬看见。<br />


可以nokvm，省事很多。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9379382&amp;ptid=760463" target="_blank"><font color="#999999">我有一个梦想 发表于 2020-10-31 09:06</font></a></font><br />
看红帽官方文档，自动分区不超过50G，不会分给/home，反之就会像你那样</blockquote></div><br />
对，就是你说的这个，不知道咋解决的

如果是自己开着玩 。那么就DD系统删swap。开IDC就不知道如何解决了。

fdisk 删掉home合进去
