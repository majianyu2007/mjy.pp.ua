# 【已解决】各位大佬，求一句SQL


<i class="pstatus"> 本帖最后由 leven5 于 2020-10-26 09:58 编辑 </i><br />
<br />
研究了好半天都不行<br />
<br />
id,name,child<br />
1,呵呵,1<br />
2,哈哈,6<br />
3,吼吼,3<br />
4,嗯嗯,4<br />
<br />
我想要如果id=child就返回A，否则返回B，命名为type<br />
<br />
我试了<br />
id,name,IF(id=child,'A','B') as type<br />
也试了<br />
id,name,CASE WHEN id=child THEN 'A' ELSE 'B' END type<br />
<br />
到底该怎么写呢？？完全不会啊<img src="static/image/smiley/yct/021.gif" smilieid="37" border="0" alt="" /> 

这写的貌似没毛病啊&nbsp;&nbsp;是不是列类型的问题<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

id,name,CASE WHEN id=child THEN 'A' ELSE 'B' END type这种没错<br />
<br />
看看是不是数据库本来就有个type列

什么都能发这里了吗？真好，SQL写判断你也是NB，不怕崩啊。。。

好好检查一下拼写

<div class="quote"><blockquote><font color="#999999">e时代无名 发表于 2020-10-26 03:26</font><br />
<font color="#999999">什么都能发这里了吗？真好，SQL写判断你也是NB，不怕崩啊。。。</font></blockquote></div><br />
就是，就是，全部拿出来。再用语言循环判断不香吗

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9352133&amp;ptid=758411" target="_blank"><font color="#999999">phpznr 发表于 2020-10-26 01:50</font></a></font><br />
id,name,CASE WHEN id=child THEN 'A' ELSE 'B' END type这种没错<br />
<br />
看看是不是数据库本来就有个type列 ...</blockquote></div><br />
确实本身有type列，不过我换了也是一样，还不行，都是全部返回A.....<br />
已经放弃了，只能全部查询了再做处理<img src="static/image/smiley/yct/021.gif" smilieid="37" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351992&amp;ptid=758411" target="_blank"><font color="#999999">518 发表于 2020-10-26 00:09</font></a></font><br />
这写的貌似没毛病啊&nbsp;&nbsp;是不是列类型的问题</blockquote></div><br />
老司机，确实啊，我又仔细看了一下，一个int一个char，cast转了一下就正确了！<br />
感谢！<img src="static/image/smiley/yct/019.gif" smilieid="49" border="0" alt="" />
