# linux服务器的内存多久清一次比较好


<i class="pstatus"> 本帖最后由 景安代理 于 2020-10-24 12:10 编辑 </i><br />
<br />
系统缓存占用比较多，在内存满了的时候不清理缓存的话会对速度影响大吗<br />
看着缓存占满了内存总想清空<br />
<img id="aimg_vDckq" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/24/GHOPiwWBcXzIkbt.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
多久清一次比较好

<i class="pstatus"> 本帖最后由 havoc06 于 2020-10-24 12:13 编辑 </i><br />
<br />
没必要清理，缓存就是为了提高性能的，真正需要使用内存的时候缓存会释放的，实在看不顺眼可以关掉，但是没必要啊

无聊！！！！！&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9345176&amp;ptid=757927" target="_blank"><font color="#999999">havoc06 发表于 2020-10-24 12:10</font></a></font><br />
有啥好清的。。缓存就是为了提高性能，实在看不顺眼可以关掉，但是没必要啊 ...</blockquote></div><br />
好，懂了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

不清理的话会杀进程的，要不你就弄个进程守护。至于清理，看你的业务了，如果杀进程就清理的勤快点，如果不杀进程，一年也不用管的

一星期一次

你一定是360手机软件重度用户
