# 子比最新4.2 体验版 怎么把页脚的版权搞掉啊？


<img id="aimg_TXOcc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/01/8v5hiJgPzUqI7xR.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
我把 framework/options-framework.php 的最后一行注释掉的话，前台确实没这句话了 可是后台主题设置直接提示文件异常了<br />
<br />
add_action('zib_footer_conter','of_auht',11);<br />


不会的话，不要自己开心，自己看下源码就知道作者做了什么验证了。

0基础人员不建议使用<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

大佬们人呢

哈哈，它会验证你文件是否有改动

搞个js 去掉 或者 反代内容替换

footer.php第七行zib_footer_conter改成zib_footer_conter1<br />
functions\zib-footer.php 109行zib_footer_conter改成zib_footer_conter1<br />
建议购买正版<img id="aimg_pKTIT" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9384830&amp;ptid=760907" target="_blank"><font color="#999999">dwf135 发表于 2020-11-1 14:12</font></a></font><br />
footer.php第七行zib_footer_conter改成zib_footer_conter1<br />
functions\zib-footer.php 109行zib_footer_con ...</blockquote></div><br />
直接 把 footer 内容 全部抹去 自己随便加点文字 会对主题 有影响吗？？？

现在不敢用什么开心版主题了 吃过亏了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9384852&amp;ptid=760907" target="_blank"><font color="#999999">guowang 发表于 2020-11-1 14:19</font></a></font><br />
直接 把 footer 内容 全部抹去 自己随便加点文字 会对主题 有影响吗？？？</blockquote></div><br />
也可以直接F12查看源代码 全部复制下来 然后删掉版权部分 粘贴到footer&nbsp;&nbsp;一样用<br />
可以正常使用&nbsp;&nbsp;有没有影响不清楚<img id="aimg_r5ucC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
