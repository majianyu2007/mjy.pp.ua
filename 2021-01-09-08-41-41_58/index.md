# .265 转 .264有什么比较好的方法


推荐GPU加速的转码，ffmpeg或者封装ffmpeg的软件都有GPU转码的

ffmpeg

<div class="quote"><blockquote><font color="#999999">不要搞我哇 发表于 2020-10-27 15:00</font><br />
<font color="#999999">格式工厂好慢，28G的转了1小时还没转完。<br />
处理器是i5-9400</font></blockquote></div><br />
转码你得加个好显卡，单靠cpu你i7也不行的。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9360409&amp;ptid=758905" target="_blank"><font color="#999999">不要搞我哇 发表于 2020-10-27 18:23</font></a></font><br />
28G视频.265转.264格式工厂转完只有18G<br />
.265不是比.264压缩率高吗？为什么转完后反而体积小了<br />
分辨率一样 ...</blockquote></div><br />
码率降了吧？<br />
分辨率。刷新率。等等参数都会导致文件大小不一样。<br />
<br />
265变264。肯定要重新计算了。。。。

硬件编码的显卡极贵，硬件解码手机都有，<br />
厂家套路，

http://www.ffmpeg.org/download.html<br />
ffmpeg -i input.mp4 -vcodec h264 output.mp4

格式工厂应该支持gpu加速，我看高级那里有，我也勾选了<br />
任务管理器里 CPU100%，GPU才2%<br />
不知道是不是版本问题，我用的是格式工厂4.9.5

得上华为的鲲服务器

我都是用小鸡转码<br />
多开几个小鸡 管他吃不吃cpu <br />
反正最多2天也转好了
