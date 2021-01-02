# 如何对日志进行按天分割


网站历史日志文件过大&nbsp;&nbsp;想对已进生成的日志文件进行按天切割，有脚本么。大佬分享下

cat access.log |grep 2020-10-23 T &gt; access-2020-10-23.log

https://**blogs.com/gosky/p/5188893.html

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9343968&amp;ptid=757818" target="_blank"><font color="#999999">Waylon 发表于 2020-10-24 00:03</font></a></font><br />
cat access.log |grep 2020-10-23 T &gt; access-2020-10-23.log</blockquote></div><br />
谢谢大佬

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9344035&amp;ptid=757818" target="_blank"><font color="#999999">Clever 发表于 2020-10-24 00:27</font></a></font><br />
谢谢大佬</blockquote></div><br />
额。这只是手动敲的分割，<br />
一天过去了，还没人给你写自动脚本吗。<img src="static/image/smiley/default/shocked.gif" smilieid="6" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349363&amp;ptid=757818" target="_blank"><font color="#999999">Waylon 发表于 2020-10-25 12:18</font></a></font><br />
额。这只是手动敲的分割，<br />
一天过去了，还没人给你写自动脚本吗。</blockquote></div><br />
自动脚本自己倒腾半天搞定了。
