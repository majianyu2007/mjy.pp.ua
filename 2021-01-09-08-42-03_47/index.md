# 火车头有没有办法采集这类网站，求解


<i class="pstatus"> 本帖最后由 baiyangz1 于 2020-10-30 14:55 编辑 </i><br />
<br />
https://www.xuexila.com/fwn/ziwojieshaomianshi/<br />
列表页只有1页，第二页就做了隐藏，<br />
<br />
只能在https://www.xuexila.com/fwn/ziwojieshaomianshi/c528661.html文章中的“下一篇”能够找到url<br />
<br />
这种模式怎么用火车头爬到所有文章URL呢，有大佬指点一下吗？<br />
<br />
解决方法：内容页循环提取分页URL，然后导出来再操作。<br />
沙比网站，还设置了反采集时间间隔，老子非要日穿它

循环采 下一页 试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375192&amp;ptid=760238" target="_blank"><font color="#999999">lanying 发表于 2020-10-30 14:40</font></a></font><br />
循环采 下一页 试试</blockquote></div><br />
好像是可以这样搞，我试试

要是我就全部抓取html。为什么一定要按顺序来。入库不就好了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375205&amp;ptid=760238" target="_blank"><font color="#999999">hxuf 发表于 2020-10-30 14:42</font></a></font><br />
要是我就全部抓取html。为什么一定要按顺序来。入库不就好了。</blockquote></div><br />
问题是怎么抓，没有索引页给你抓啊，而且这是分专题的，很难搞。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9375213&amp;ptid=760238" target="_blank"><font color="#999999">baiyangz1 发表于 2020-10-30 14:44</font></a></font><br />
问题是怎么抓，没有索引页给你抓啊，而且这是分专题的，很难搞。</blockquote></div><br />
直接循环抓取所有html啊。

必须可以
