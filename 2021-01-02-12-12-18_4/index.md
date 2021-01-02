# 求个mysql语句


id&nbsp; &nbsp;name<br />
1&nbsp; &nbsp; 张三<br />
2&nbsp; &nbsp; 李四<br />
3&nbsp; &nbsp; 王五<br />
4&nbsp; &nbsp; 赵六<br />
<br />
需要把name 转换成 张三1 李四2 王五3&nbsp;&nbsp;也就是把列的id加在name后面&nbsp;&nbsp;请教下该怎么写！求大佬指点！

concat(name,id) as name

我等大佬们回答了来看看答案<br />
<br />
学习下知识！<br />
<br />
帮顶！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

我也不懂

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9339609&amp;ptid=757484" target="_blank"><font color="#999999">ttzpp 发表于 2020-10-23 09:53</font></a></font><br />
concat(name,id) as name</blockquote></div><br />
得循环处理吗？

楼上正解 update 表名 set `name`= concat(`name`, id)

用union就好了，具体语句可百度：SQL 列合并

小意思！<div class="blockcode"><div id="code_X02"><ol><li>UPDATE TableName<br /><li>SET NAME = REPLACE (<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; NAME,<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; '@id',<br /><li>&nbsp; &nbsp; &nbsp; &nbsp;&nbsp;&nbsp;CONCAT('@id(description =&quot;',TableName,'&quot;)') ) ;</ol></div><em onclick="copycode($('code_X02'));">复制代码</em></div>

解决了 多谢楼上大佬

学习了~~ 我之前也发过mysql的问题帖，由于数据太大，一直没有解决方法
