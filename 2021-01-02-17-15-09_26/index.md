# 请教php大佬 foreach循环中能插入数据么


想在foreach输出第一个数组元素时插入个元素，搜了下貌似没相关代码&nbsp; &nbsp;是foreach没法计数吗。。<br /><div class="blockcode"><div id="code_t4z"><ol><li>&lt;?php <br /><li>$colors = array(&quot;red&quot;,&quot;green&quot;,&quot;blue&quot;,&quot;yellow&quot;); <br /><li><br /><li>foreach ($colors as $value) {<br /><li>&nbsp; &nbsp;echo &quot;$value &lt;br&gt;&quot;;<br /><li>}<br /><li>?&gt;&nbsp; &nbsp;</ol></div><em onclick="copycode($('code_t4z'));">复制代码</em></div>

帮顶<br />
<br />
技术大佬们回答吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

foreach (array_expression as $key =&gt; $value)&nbsp;&nbsp;<br />
文档看下

外面定义一个 i&nbsp; &nbsp; foreach&nbsp;&nbsp;里面 i++&nbsp; &nbsp;&nbsp;&nbsp;判断 i == 1&nbsp; &nbsp;这样子也行

输出第一个数组元素时插入个元素?<br />
<br />
这句话是什么意思&nbsp; &nbsp; 没看懂&nbsp; &nbsp;最好举个例子来解释<br />


你自己定义一个临时变量来计数不就得了？<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />，例如上面的定义i ，用i++<img id="aimg_S5Faf" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351275&amp;ptid=758377" target="_blank"><font color="#999999">alk19t 发表于 2020-10-25 21:07</font></a></font><br />
输出第一个数组元素时插入个元素?<br />
<br />
这句话是什么意思&nbsp; &nbsp; 没看懂&nbsp; &nbsp;最好举个例子来解释</blockquote></div><br />
就是循环第一个元素时，比如red，这时就额外插入元素x<br />
我试试上面大佬的方法

<div class="blockcode"><div id="code_RgF"><ol><li>&lt;?php<br /><li>$colors = array(&quot;red&quot;,&quot;green&quot;,&quot;blue&quot;,&quot;yellow&quot;);<br /><li><br /><li>foreach ($colors as $k=&gt;$v) {<br /><li>&nbsp; &nbsp;&nbsp;&nbsp;$colors[$k] .= &quot;fuck&quot;;<br /><li>}<br /><li>?&gt;&nbsp; &nbsp;</ol></div><em onclick="copycode($('code_RgF'));">复制代码</em></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351313&amp;ptid=758377" target="_blank"><font color="#999999">duyu 发表于 2020-10-25 21:15</font></a></font></blockquote></div><br />
<br />
多谢大佬，这个会循环输出4个fuck，能帮忙改下吗<br /><div class="blockcode"><div id="code_x6a"><ol><li>array(4) {<br /><li>&nbsp;&nbsp;[0]=&gt;<br /><li>&nbsp;&nbsp;string(19) &quot;redfuckfuckfuckfuck&quot;<br /><li>&nbsp;&nbsp;[1]=&gt;<br /><li>&nbsp;&nbsp;string(5) &quot;green&quot;<br /><li>&nbsp;&nbsp;[2]=&gt;<br /><li>&nbsp;&nbsp;string(4) &quot;blue&quot;<br /><li>&nbsp;&nbsp;[3]=&gt;<br /><li>&nbsp;&nbsp;string(6) &quot;yellow&quot;<br /><li>}</ol></div><em onclick="copycode($('code_x6a'));">复制代码</em></div>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351328&amp;ptid=758377" target="_blank"><font color="#999999">guoaibing 发表于 2020-10-25 21:24</font></a></font><br />
多谢大佬，这个会循环输出4个fuck，能帮忙改下吗</blockquote></div><br />
<div class="blockcode"><div id="code_a7J"><ol><li>&lt;?php<br /><li>$colors = array(&quot;red&quot;,&quot;green&quot;,&quot;blue&quot;,&quot;yellow&quot;);<br /><li><br /><li>foreach ($colors as $k=&gt;$v) {<br /><li>&nbsp; &nbsp;&nbsp;&nbsp;$colors[0] .= &quot;fuckfuckfuckfuck&quot;;<br /><li>}<br /><li>?&gt;&nbsp; &nbsp;</ol></div><em onclick="copycode($('code_a7J'));">复制代码</em></div><br />
<br />
这样好像也没必要用foreach啊
