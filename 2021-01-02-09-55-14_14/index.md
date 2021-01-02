# iplc的内网延迟怎么测


rt<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> 

从一端ping另一端的内网ip<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333313&amp;ptid=756931" target="_blank"><font color="#999999">zenghaochen 发表于 2020-10-21 21:14</font></a></font><br />
从一端ping另一端的内网ip</blockquote></div><br />
商家只给了一个内网地址，我怎么判断这个内网地址是哪台鸡的···

ping一下就知道了，一般本地不会超过1ms<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333334&amp;ptid=756931" target="_blank"><font color="#999999">zenghaochen 发表于 2020-10-21 21:18</font></a></font><br />
ping一下就知道了，一般本地不会超过1ms</blockquote></div><br />
谢谢大佬<br />
已知的内网地址是本机的···没有另外一台鸡的内网地址，还有方法测内网延迟吗

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9333346&amp;ptid=756931" target="_blank"><font color="#999999">asdii 发表于 2020-10-21 21:21</font></a></font><br />
谢谢大佬<br />
已知的内网地址是本机的···没有另外一台鸡的内网地址，还有方法测内网延迟吗 ...</blockquote></div><br />
ifconfig看看本地所有网卡的地址，如果只有一个的话那就超出我的知识范围了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

把内网ip同一网段下所有ip都ping一遍就完事了吧<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

看看你的iplc是不是显示真实ip，不显示的话源ip就是入口ip

ping 下出口机的IP
