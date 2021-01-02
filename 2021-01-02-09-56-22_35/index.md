# 问个shell命令的问题。


我有一些代码。每次用xshell 有3段命令，每次复制全部执行，我想合在一起弄个sh脚本的话。<br />
是里面的所有关于路径的，都要写绝对路径么。目前有不成功的时候，不知道哪里问题。

如果你不能确保工作路径的话那你最好用绝对路径

请技术大佬们回答吧！<br />
<br />
我直接帮楼主说谢谢！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451241&amp;ptid=766446" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-13 23:50</font></a></font><br />
请技术大佬们回答吧！<br />
<br />
我直接帮楼主说谢谢！</blockquote></div><br />
肯定不是F5刷的。跟我发帖相差不到50秒啊。。。又拼字。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451249&amp;ptid=766446" target="_blank"><font color="#999999">斌斌 发表于 2020-11-13 23:51</font></a></font><br />
肯定不是F5刷的。跟我发帖相差不到50秒啊。。。又拼字。</blockquote></div><br />
你不信我也没办法！<br />
<br />
我每个帖子回复，都是手动刷新，然后手动打字！<br />
<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451265&amp;ptid=766446" target="_blank"><font color="#999999">最美嫦娥颜丹晨 发表于 2020-11-13 23:55</font></a></font><br />
额 你不能决定工作路径的话那就只能写绝对路径 不然就得搞通配符出来</blockquote></div><br />
如果没有这个命令的话，还会继续向下执行么。比如这个，有的centos7就没有这命令。<br />
systemctl stop firewalld.service

没有命令直接报错，路径是按照你执行这个脚本的路径为基础的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451285&amp;ptid=766446" target="_blank"><font color="#999999">斌斌 发表于 2020-11-13 23:59</font></a></font><br />
如果没有这个命令的话，还会继续向下执行么。比如这个，有的centos7就没有这命令。<br />
systemctl stop firew ...</blockquote></div><br />
<br />
只要脚本<u>符合语法</u>就会一直运行下去

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451285&amp;ptid=766446" target="_blank"><font color="#999999">斌斌 发表于 2020-11-13 23:59</font></a></font><br />
如果没有这个命令的话，还会继续向下执行么。比如这个，有的centos7就没有这命令。<br />
systemctl stop firew ...</blockquote></div><br />
默认中途出错继续执行，但是会输出错误提示
