# 求教大佬标签语法问题


img标签<br />
<br />
<img id="aimg_Qqfn6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/27/BMANLV.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
这两种写法哪种正确？还是说都正确？<br />
<br />
alt 和 title 可否同时使用？ 哪个在前哪个在后有没有要求？

多个斜杠是标准写法

title没啥意义，它主要是给超链接a用的。

都可以，对seo没啥影响，你就多个斜杠而已，不过既然是图片<br />
建议你每个alt和title，后面分一，二，三，或者图一，图二，图三，而不是都是一个标题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9357301&amp;ptid=758827" target="_blank"><font color="#999999">战神赵日天 发表于 2020-10-27 08:50</font></a></font><br />
都可以，对seo没啥影响，你就多个斜杠而已，不过既然是图片<br />
建议你每个alt和title，后面分一，二，三，或者 ...</blockquote></div><br />
多谢大佬指点迷津

标签有开闭才符合标准，2是对的

多斜杠是标准写法。 代表标签关闭。

<i class="pstatus"> 本帖最后由 yousihai 于 2020-10-27 10:09 编辑 </i><br />
<br />
img标签不需要闭合。所以第一个是准确的，当然第二个也没问题<br />
<br />
https://stackoverflow.com/questions/23890716/why-is-the-img-tag-not-closed-in-html<br />
<br /><div class="quote"><blockquote>Historically, HTML has been based on SGML which allows tags to be omitted under certain conditions.<br />
<br />
Since the 《img》 element cannot have any child nodes, it is defined as EMPTY and the end tag is forbidden (as it would serve no purpose).<br />
<br />
XHTML is HTML expressed in XML, and XML does not support optional or forbidden tags (although it allows a self-closing tag to substitute for a start+end tag pair), so it has to be explicitly closed there.<br />
<br />
HTML 5 is backwards compatible with versions of HTML that were SGML based.</blockquote></div>

感谢楼上几位大佬的指点
