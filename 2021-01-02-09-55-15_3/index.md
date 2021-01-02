# Debian10下面的mariadb表总是崩溃


哈哈，不会做站<br />
<br />
没遇到过！不行换9用吧！<br />
<br />
9也挺好用的啊！<br />
<br />
<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

这个不怎么清楚。

vps 内存太少，试试开 swap 试试<br />
我上次香港AZ，800M内存，开swap 才把 数据库开起来

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9334965&amp;ptid=757066" target="_blank"><font color="#999999">查无此人 发表于 2020-10-22 10:47</font></a></font><br />
3900xt M2 ddr4 16G</blockquote></div><br />
这么好的配置，就应该要优化数据和SQL语句了<br />
这些就要专业的人处理了

这个时候就怀疑是设置的问题了

使用的是innoDB引擎？

建议导入并使用 mysql8.0

内存太小
