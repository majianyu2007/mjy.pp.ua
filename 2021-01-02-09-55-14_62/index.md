# 求ffmpeg h264转h265的命令


网上能搜到但是怕有坑，事关1.x PB大姐姐身家性命，请大佬给个靠谱的命令参数。<br />
<br />
听说GD在砍盘，还是放自己服务器上吧。<br />
<br />
CPU转码h264到h265，是不是可以做到画质肉眼看不到区别？

参数调整不当会导致画质下降或者体积变大，得不偿失

1.x PB? 1xxx TB?<br />
平均一部4G，一共250000部，时长一小时的，CPU Xeon 12 Core H.264-&gt;H.265 ffmpeg 平均 1800秒/部，也就是半个小时一部。<br />
<br />
250000*0.5/24=5208天，转码10多年？

卧槽，1.X&nbsp;&nbsp;PB的DJJ，这是要精尽人亡啊！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

先借一部说话？

H265好像是没有H264通用吧？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333444&amp;ptid=756940" target="_blank"><font color="#999999">疯狂痴呆 发表于 2020-10-21 21:41</font></a></font><br />
H265好像是没有H264通用吧？</blockquote></div><br />
只要能在同画质下降低容量，其他的不考虑。

我也有过类似的想法，但是经过调查之后，发现转码不仅时间成本太高了，压缩必然有损失，省下来空间并不大。还是剪掉不喜欢的某个片段比较合适，省空间也省时间

还有搞两个不同域名的gd，同步备份，也可以降低一部分风险

转码太费时间和算力了吧

<div class="blockcode"><div id="code_X32"><ol><li>使用 FFMPEG 转 H265 减小文件大小<br /><li>ffmpeg -i input.mp4 -c:v libx265 -crf 30 -map 0:v -map 0:a:0 output.mp4 <br /><li><br /><li>crf越高,压缩率越高,值是30-100</ol></div><em onclick="copycode($('code_X32'));">复制代码</em></div>
