# 请教python如何从mysql读取数据转换成account_dict


目前python在用以下格式<br />
account_dict = {<br />
&nbsp; &nbsp; '0': {'字段1': 'aaa', '字段2: 'vvv', '字段3': '4434'},<br />
&nbsp; &nbsp; '1': {'字段1': 'dsf', '字段2: '325', '字段3': '4224'},<br />
&nbsp; &nbsp; '2': {'字段1': 'b4d', '字段2: 'k87', '字段3': '6224'},<br />
&nbsp; &nbsp; '3': {'字段1': '54g', '字段2: 'v5v', '字段3': '8788'},<br />
&nbsp; &nbsp; '4': {'字段1': 'h65', '字段2: '434', '字段3': '4774'},<br />
<br />
}<br />
<br />
但是不便于管理，想从mysql读取数据，目前pymysql都正常，也能连接数据库，也能读取文件，就是不知道如何转变成account_dict 的格式，所以请大佬们指点下，该从哪里入手学习，有什么关键词可以去谷歌或者百度搜索<br />
<br />
<br />
假如我的mysql字段如下<br />
字段1&nbsp; &nbsp; &nbsp; &nbsp; 字段2&nbsp; &nbsp; &nbsp; &nbsp; 字段3<br />
kj8&nbsp; &nbsp; &nbsp; &nbsp; dsdsa&nbsp; &nbsp; &nbsp; &nbsp; 42332<br />
dsk&nbsp; &nbsp; &nbsp; &nbsp; dasd&nbsp; &nbsp; &nbsp; &nbsp; 23<br />
k02&nbsp; &nbsp; &nbsp; &nbsp; 323&nbsp; &nbsp; &nbsp; &nbsp; 43<br />
jvf&nbsp; &nbsp; &nbsp; &nbsp; 21f&nbsp; &nbsp; &nbsp; &nbsp; 656<br />
mjs&nbsp; &nbsp; &nbsp; &nbsp; 21&nbsp; &nbsp; &nbsp; &nbsp; 3453<br />
ke0&nbsp; &nbsp; &nbsp; &nbsp; 424&nbsp; &nbsp; &nbsp; &nbsp; 656<br />
k28&nbsp; &nbsp; &nbsp; &nbsp; 54&nbsp; &nbsp; &nbsp; &nbsp; 43<br />
<br />


可以自己构造一下

估计没啥好办法，查出来自己组装下吧<img src="static/image/smiley/default/titter.gif" smilieid="9" border="0" alt="" />

Flask-SQLAlchemy

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9362826&amp;ptid=759293" target="_blank"><font color="#999999">MikuSama 发表于 2020-10-28 10:21</font></a></font><br />
Flask-SQLAlchemy</blockquote></div><br />
多谢，这就去研究研究

你这account dict也太优秀了，不会用list？
