# 大佬们，正则正则正则，帮个忙。


<i class="pstatus"> 本帖最后由 baijia7758 于 2020-11-25 10:52 编辑 </i><br />
<br />
C:\\\\Users\\\\i\\\\\\\\\\\Desktop\\\\\\\\\\\\\新建文件夹\\\\\\\\\\\\<br />
<br />
<br />
怎么将 多个 \\\\ 替换成 一个 \ 或两个 \\<br />
<br />
<br />
C://///Users////i////Desktop////新建文件夹////////<br />
<br />
怎么将 多个 ////替换成 一个 /<br />
<br />
<img src="static/image/smiley/default/sweat.gif" smilieid="10" border="0" alt="" /> <br />
<br />
大佬未出现，搞定了<div class="blockcode"><div id="code_qv5"><ol><li>([\\])(\1*)</ol></div><em onclick="copycode($('code_qv5'));">复制代码</em></div> <img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> 

笑出声，这原始字符串到底经历了什么

迷惑行为<br />
这点事还要正则<br />
记事本&nbsp;&nbsp;替换 \\ 为 \ 多点两次全部替换搞定

查找/+，替换为/或//

没看懂，大佬能解释一下吗？<br />
[\\] 这个就很奇怪了，两个\ 任何一个？<br />
(\1*) 分组1 然后*什么意思？<br />
<br />
ps. 这是python 的正则吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9513851&amp;ptid=771102" target="_blank"><font color="#999999">qanniu 发表于 2020-11-25 11:12</font></a></font><br />
没看懂，大佬能解释一下吗？<br />
[\\] 这个就很奇怪了，两个\ 任何一个？<br />
(\1*) 分组1 然后*什么意思？</blockquote></div><br />
<br />
单个\不能输入呀，转义字符 \\ 是 \<br />
<br />
后面不能回答你 了，我是瞎蒙调试出来的。看了很多资料哈哈 ，不懂正则。

牛批，学习下<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> 。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9513851&amp;ptid=771102" target="_blank"><font color="#999999">qanniu 发表于 2020-11-25 11:12</font></a></font><br />
没看懂，大佬能解释一下吗？<br />
[\\] 这个就很奇怪了，两个\ 任何一个？<br />
(\1*) 分组1 然后*什么意思？</blockquote></div><br />
\\是第一个\对第二个\进行转义，代表就匹配\本身。对于题主的问题 我觉得正则写成(\\)+ 然后替换成\ 就可以了吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9514075&amp;ptid=771102" target="_blank"><font color="#999999">ivanhao 发表于 2020-11-25 11:37</font></a></font><br />
\\是第一个\对第二个\进行转义，代表就匹配\本身。对于题主的问题 我觉得正则写成(\\)+ 然后替换成\ 就可 ...</blockquote></div><br />
（\\+）
