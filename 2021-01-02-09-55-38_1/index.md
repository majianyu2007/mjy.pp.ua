# 有大佬知道这个怎么排查解决吗


wordpress 不知道怎么了 更新还是啥 就成这样了<br />
<br />
<img id="aimg_KjXoE" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="72" src="https://p.pstatp.com/origin/1000000027081cf780670.jpg" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
查看是多了这个<br />
<img id="aimg_FmWSS" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="72" src="https://p.pstatp.com/origin/ff74000335527ef41539.jpg" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
有什么排查方法吗<img id="aimg_UMPDE" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 sh3dowin 于 2020-10-24 20:42 编辑 </i><br />
<br />
这个文件 wp-content/themes/kratos/assets/css/kratos.min.css?ver=3.2.0<br />
搜 .k-header .banner {<br />
<br />
改为<br />
<br /><div class="blockcode"><div id="code_Nrr"><ol><li>.k-header .banner {<br /><li>&nbsp; &nbsp; position: relative;<br /><li>&nbsp; &nbsp; height: 300px;<br /><li>&nbsp; &nbsp; bottom: 28px;<br /><li>}</ol></div><em onclick="copycode($('code_Nrr'));">复制代码</em></div>

帮顶，来个前端大佬！<br />
<br />
回答一下！<br />
<br />
小白路过！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

空格符号而已，你是强迫症吗

bom的问题，好像编辑源码要去bom就解决了

php代码里面对应位置的空格删掉<img id="aimg_l6F20" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347146&amp;ptid=758055" target="_blank"><font color="#999999">zaeve 发表于 2020-10-24 19:24</font></a></font><br />
php代码里面对应位置的空格删掉</blockquote></div><br />
我把整站源码down下来 没找到有这个的<img id="aimg_fc7p4" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

我不行你们来吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347141&amp;ptid=758055" target="_blank"><font color="#999999">星空下的祈愿 发表于 2020-10-24 19:22</font></a></font><br />
空格符号而已，你是强迫症吗</blockquote></div><br />
你看我签名站的效果 不对劲啊<img id="aimg_To0JK" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347142&amp;ptid=758055" target="_blank"><font color="#999999">fifalan 发表于 2020-10-24 19:23</font></a></font><br />
bom的问题，好像编辑源码要去bom就解决了</blockquote></div><br />
谢谢，我试试<img id="aimg_KbB5c" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 小小白 于 2020-10-24 20:10 编辑 </i><br />
<br />
1111111
