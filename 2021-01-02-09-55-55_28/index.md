# 用python下载PH上的学习视频


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9400008&amp;ptid=762053" target="_blank"><font color="#999999">海苔 发表于 2020-11-4 10:29</font></a></font><br />
python的多线程不是残废吗，多进程好点吧，request可以加个重试好点</blockquote></div><br />
非计算密集型，用多线程也可以<br />
进程开销比较大，扔垃圾小鸡上跑，估计提升不了多少

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9400025&amp;ptid=762053" target="_blank"><font color="#999999">laogui 发表于 2020-11-4 10:32</font></a></font><br />
优先选择 1080P&gt;720P&gt;480P<br />
如果视频源没这三分辨率，跳过下载</blockquote></div><br />
厉害了，点赞！

所有你是直接源代码拼接的？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9400004&amp;ptid=762053" target="_blank"><font color="#999999">laogui 发表于 2020-11-4 10:27</font></a></font><br />
我也是菜鸟，刚学的python<br />
目前只知道从JS代码中的flashvars_xxxxxxxxx变量中解析获取视频链接 ...</blockquote></div><br />
目前我大概能下了。.net core效率超py

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9400950&amp;ptid=762053" target="_blank"><font color="#999999">peng123 发表于 2020-11-4 12:34</font></a></font><br />
所有你是直接源代码拼接的？</blockquote></div><br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
它的视频链接是在JS里拼接的，具体存在flashvars_xxxxxxxxx变量中<br />
用python把相关变量提取出来再拼接
