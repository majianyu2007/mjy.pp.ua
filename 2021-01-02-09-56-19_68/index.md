# 大佬们，U盘突然不能制作启动盘了，啥情况


之前都能制作，优启通使用很好，前段时间突然<font color="Red"><strong>偶尔</strong></font>不能成功启动，也没管，以为是接触不良。<br />
<br />
最近装一个pve，就格式化了，ultraiso，Ethcher，img32什么什么的软件都试过，就是死活不能启动，还以为是电脑主板问题。<br />
<br />
终于用另外一个优盘，成功安装了。<br />
<br />
问题来了，同样的软件，同样的方法，同样iso，同样的主板，我的U盘制作的启动盘就是不能识别。<br />
<br />
win的diskpart，clean命令都用过了，在win10上可以正常识别，存取，分区，就是制作启动盘不成功！！！<br />
<br />
有没有大佬碰到过，到底啥问题

爱国者就是辣鸡，8层是爱国者U盘出现问题了<br />
<br />
建议申请售后或者退款换闪迪吧

它老了，需要退休！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449303&amp;ptid=766298" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-13 16:59</font></a></font><br />
它老了，需要退休！</blockquote></div><br />
去年才买的U盘，爱国者32G

烧录有风险的，容易坏。

使用&nbsp;&nbsp;DiskGenius&nbsp;&nbsp;看看分区情况，把U盘分区删除掉试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449309&amp;ptid=766298" target="_blank"><font color="#999999">michelleman 发表于 2020-11-13 17:01</font></a></font><br />
去年才买的U盘，爱国者32G</blockquote></div><br />
爱国者一般出了质保期，就不太行了！<br />
<br />
一年质保，一年工作寿命！<br />
<br />
<img src="static/image/smiley/default/loveliness.gif" smilieid="28" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449317&amp;ptid=766298" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-13 17:02</font></a></font><br />
爱国者一般出了质保期，就不太行了！<br />
<br />
一年质保，一年工作寿命！</blockquote></div><br />
问题是当个普通优盘存取文件完全没问题，想不通原理啊

用工具重新做或者格式化成FAT32，自己导入引导文件

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449331&amp;ptid=766298" target="_blank"><font color="#999999">michelleman 发表于 2020-11-13 17:05</font></a></font><br />
问题是当个普通优盘存取文件完全没问题，想不通原理啊</blockquote></div><br />
好像是用做启动，需要读取最开始几个扇区<br />
<br />
具体我也不太懂！存存数据吧！

油漆桶还原空间，再用旧版的试试。
