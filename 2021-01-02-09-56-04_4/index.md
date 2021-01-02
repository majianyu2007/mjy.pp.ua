# 数据库更新命令语法怎么写？？大佬进


<i class="pstatus"> 本帖最后由 baiyangz1 于 2020-11-5 12:21 编辑 </i><br />
<br />
数据库是mysql，在宝塔后台phpmyadmin那边执行操作的。<br />
<br />
需求：在表一中，字段1中，其中的字符串，aaa.com/picture/2020/11/（这里的年份和月份不是固定的）替换成bbb.com/picture/2020/10/（这里的年份和月份是固定的）<br />
<br />
补充：试过了普通的update 表名 set 字段名 =replace(字段名,&quot;aaa.com/picture/%/%/&quot;,&quot;bbb.com/picture/2020/10/&quot;)，不行，replace不能用通配符。

如果你的mysql版本较高，可以用regexp_replace，这个可以正则匹配。

<i class="pstatus"> 本帖最后由 论坛大师 于 2020-11-5 09:27 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404940&amp;ptid=762621" target="_blank"><font color="#999999">baiyangz1 发表于 2020-11-5 09:13</font></a></font><br />
数据库是sql，在宝塔后台phpmyadmin那边执行操作的。</blockquote></div><br />
<br />
phpmyadmin是不支持sql数据库的，你需要这个 https://www.microsoft.com/zh-cn/sql-server/sql-server-downloads<img id="aimg_ArIPX" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

什么数据库，几十种呢

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404932&amp;ptid=762621" target="_blank"><font color="#999999">l516q 发表于 2020-11-5 09:11</font></a></font><br />
什么数据库，几十种呢</blockquote></div><br />
数据库是sql，在宝塔后台phpmyadmin那边执行操作的。

给我开个权限&nbsp;&nbsp;我去给你更了 <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<i class="pstatus"> 本帖最后由 xnlebb 于 2020-11-5 09:36 编辑 </i><br />
<br />
先备份再试<br />
update 表名 set 字段名='bbb.com/picture/2020/10/' where 字段名 regexp 'aaa.com/picture/[[:digit:]]{4}/[[:digit:]]{2}/'<br />
参考 https://blog.csdn.net/vvhesj/article/details/22299413

数据量不多的话，实在不行就随便找个语言写个脚本，数据分批取出来，修改完再丢回去

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404995&amp;ptid=762621" target="_blank"><font color="#999999">论坛大师 发表于 2020-11-5 09:26</font></a></font><br />
phpmyadmin是不支持sql数据库的，你需要这个 https://www.microsoft.com/zh-cn/sql-server/sql-server-do ...</blockquote></div><br />
搞错了，是mysql，我不是很懂这些<img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" />

你直接用pma的替换功能，生成语句就可以。可以用通配符

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9405016&amp;ptid=762621" target="_blank"><font color="#999999">baiyangz1 发表于 2020-11-5 09:28</font></a></font><br />
搞错了，是mysql，我不是很懂这些</blockquote></div><br />
MySQL就说MySQL，SQL是指微软公司的 Server SQL<img id="aimg_A1U8r" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
