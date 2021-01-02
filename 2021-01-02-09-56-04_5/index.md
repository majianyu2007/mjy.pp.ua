# 数据库更新命令语法怎么写？？大佬进


先备份<br />
UPDATE 表名 SET 字段名 = 'bbb.com/picture/2020/10/' WHERE 字段名 LIKE 'aaa.com/picture/%/%/';<br />
这样可以吗

知识错误了<br />
<br />
这种基础问题直接搜索一下即可<br />
<br />
问反而耗费时间

<div class="blockcode"><div id="code_I55"><ol><li>update `表名` set `字段名` = &quot;bbb.com/picture/2020/10/&quot; where `字段名 ` regexp &quot;aaa.com/picture/[0-9]+/[0-9]+/&quot;</ol></div><em onclick="copycode($('code_I55'));">复制代码</em></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405011&amp;ptid=762621" target="_blank"><font color="#999999">傍晚升起的太阳 发表于 2020-11-5 09:27</font></a></font><br />
数据量不多的话，实在不行就随便找个语言写个脚本，数据分批取出来，修改完再丢回去 ...</blockquote></div><br />
我主要是想知道方法，本办法肯定有。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404991&amp;ptid=762621" target="_blank"><font color="#999999">xnlebb 发表于 2020-11-5 09:25</font></a></font><br />
先备份再试<br />
update 表名 set 字段名='bbb.com/picture/2020/10/' where 字段名 regexp 'aaa.com/picture/[[ ...</blockquote></div><br />
感谢哈，但是这样会把整个字段变成bbb.com/picture/2020/10/，里面其实还有很多其他内容。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405036&amp;ptid=762621" target="_blank"><font color="#999999">论坛大师 发表于 2020-11-5 09:30</font></a></font><br />
MySQL就说MySQL，SQL是指微软公司的 Server SQL</blockquote></div><br />
微软公司的 Server SQL&nbsp;&nbsp;是&nbsp;&nbsp;mssql

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405155&amp;ptid=762621" target="_blank"><font color="#999999">baiyangz1 发表于 2020-11-5 09:50</font></a></font><br />
感谢哈，但是这样会把整个字段变成bbb.com/picture/2020/10/，里面其实还有很多其他内容。 ...</blockquote></div><br />
你建个账号给我啊 弄个临时表&nbsp; &nbsp;我去给你更好了 就把语句给你 

你 使用update语句的时候where条件内直接 字段 like 'aaa.com/picture/%'不就好了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405174&amp;ptid=762621" target="_blank"><font color="#999999">class 发表于 2020-11-5 09:53</font></a></font><br />
微软公司的 Server SQL&nbsp;&nbsp;是&nbsp;&nbsp;mssql</blockquote></div><br />
是的，但是单说sql服务器就是指mssql，搞运维的都这样叫<img id="aimg_QDUyD" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

下载成sql，然后notepad++一把梭
