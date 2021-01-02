# 求ffmpeg h264转h265的命令


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333820&amp;ptid=756940" target="_blank"><font color="#999999">开倒车 发表于 2020-10-21 23:14</font></a></font><br />
头次看到，研究下。<br />
顺便求下转码命令。</blockquote></div><br />
我不懂呀，我就是拿来吹牛逼。<br />
我是前段时间看到 h.266 https://zh.wikipedia.org/wiki/VVC 出来了拿来跟 av1 比才知道 av1 这个编码的。<br />
不过 VVC 年中才发布，av1 现在有很多大厂在上了 有图比 netflix 爱奇艺 推特 都在切换到 av1。

头一次听说这么猛的大兄弟，计算量太大了，真不划算

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333820&amp;ptid=756940" target="_blank"><font color="#999999">开倒车 发表于 2020-10-21 23:14</font></a></font><br />
头次看到，研究下。<br />
顺便求下转码命令。</blockquote></div><br />
建议用svt-av1.ffmpeg自带的libaom-av1好慢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9334066&amp;ptid=756940" target="_blank"><font color="#999999">achemg 发表于 2020-10-22 00:26</font></a></font><br />
建议用svt-av1.ffmpeg自带的libaom-av1好慢</blockquote></div><br />
发现了，慢的一塌糊涂。<br />
<br />
svt-av1这个画质会有影响吗？

<div class="quote"><blockquote><font color="#999999">yidaomm 发表于 2020-10-21 23:00</font><br />
<font color="#999999">如果 ffmpeg h265转h264<br />
也同样用此命令么~~</font></blockquote></div><br />
libx265 是CPU软件编码，如果本地硬件gpu编码是另一个。

<div class="quote"><blockquote><font color="#999999">开倒车 发表于 2020-10-22 00:38</font><br />
<font color="#999999">发现了，慢的一塌糊涂。<br />
<br />
svt-av1这个画质会有影响吗？</font></blockquote></div><br />
没什么影响，但svt–av1在同等画质下，编出来的码率稍高些。不过稍高的码率换快的多速度还是值的

这绝对开站的

大佬也是down的DMM???<br />
1.3PB多的？<br />
我目前也在把这1.3PB由H264转成H265，不过我为了省空间，还稍微降低了码率

大佬，求SSSSVIP

画质不下降，容量一半
