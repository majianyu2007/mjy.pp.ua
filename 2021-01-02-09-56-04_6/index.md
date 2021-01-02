# 数据库更新命令语法怎么写？？大佬进


<i class="pstatus"> 本帖最后由 xnlebb 于 2020-11-5 11:06 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405155&amp;ptid=762621" target="_blank"><font color="#999999">baiyangz1 发表于 2020-11-5 09:50</font></a></font><br />
感谢哈，但是这样会把整个字段变成bbb.com/picture/2020/10/，里面其实还有很多其他内容。 ...</blockquote></div><br />
<br />
update 表名 set 字段名=regexp_replace(字段名, 'aaa.com/picture/[[:digit:]]{4}/[[:digit:]]{2}/', 'bbb.com/picture/2020/10/')

如果你的mysql版本较高，可以用regexp_replace，这个可以正则匹配。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405480&amp;ptid=762621" target="_blank"><font color="#999999">xnlebb 发表于 2020-11-5 10:41</font></a></font><br />
update 表名 set 字段名=regexp_replace(字段名, 'aaa.com/picture/[[:digit:]]{4}/[[:digit:]]{2}/', 'b ...</blockquote></div><br />
谢啦，大佬<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
