# 请人改个代码，人民币200元


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9330136&amp;ptid=756625" target="_blank"><font color="#999999">jacksh 发表于 2020-10-21 09:41</font></a></font><br />
spf dkim都有做，就是文本这里扣分。</blockquote></div><br />
您发的邮件是包含html内容的吧？如果是，照那的问答来看，是需要在邮件头里加上mime的，如<div class="blockcode"><div id="code_D8A"><ol><li>$headers&nbsp;&nbsp;.= 'MIME-Version: 1.0' . &quot;\r\n&quot;;</ol></div><em onclick="copycode($('code_D8A'));">复制代码</em></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9331332&amp;ptid=756625" target="_blank"><font color="#999999">LiuJia 发表于 2020-10-21 13:43</font></a></font><br />
您发的邮件是包含html内容的吧？如果是，照那的问答来看，是需要在邮件头里加上mime的，如&nbsp;&nbsp;...</blockquote></div><br />
我就一小白，不懂代码的，大佬能帮改下吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9331594&amp;ptid=756625" target="_blank"><font color="#999999">小鱼 发表于 2020-10-21 14:47</font></a></font><br />
调到满分很容易啊</blockquote></div><br />
来来来，帮我调下，给辛苦费&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9331644&amp;ptid=756625" target="_blank"><font color="#999999">老坛酸菜 发表于 2020-10-21 14:54</font></a></font><br />
有人改么？</blockquote></div><br />
还没，可能钱太少了，大佬看不上吧&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;

在 sendmail.jsp 第46行 action='' 后添加 enctype=&quot;text/plain&quot;<br />
<br />
完整代码如下 <br />
&lt;form name='mailForm' action='' enctype=&quot;text/plain&quot;&gt;<br />
<br />
试试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9331765&amp;ptid=756625" target="_blank"><font color="#999999">fgpgy 发表于 2020-10-21 15:12</font></a></font><br />
在 sendmail.jsp 第46行 action='' 后添加 enctype=&quot;text/plain&quot;<br />
<br />
完整代码如下 </blockquote></div><br />
试了，一样的扣1.8分，两个扣分项没变过。&nbsp; &nbsp;&nbsp; &nbsp;

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9331594&amp;ptid=756625" target="_blank"><font color="#999999">小鱼 发表于 2020-10-21 14:47</font></a></font><br />
调到满分很容易啊</blockquote></div><br />
大佬，联系我啊，改好后领钱<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;
