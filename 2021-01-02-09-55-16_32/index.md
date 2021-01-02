# 这种刷新一次变换一次图片是怎么做的？


http://img.qqshi.com/uploadfile/202010/19/2020101915113614029.jpg<img id="aimg_eaMoE" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 hjvn2211445 于 2020-10-22 14:59 编辑 </i><br />
<br />
api.diskgirl.com/image/api.php<br />
<br />
<img id="aimg_cfwj6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://api.diskgirl.com/image/api.php" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

改的后缀。。。

这是伪静态搞出来的吗？

rewrite的网址<br />
实际上是一个程序 img.php?id=202010/19/2020101915113614029<img id="aimg_w1cCY" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

php js都能做这种随机图片啊

好多年前贴吧就流行这种回复一次就刷新一次的图片，PHP通过readfile输出的一个header为image/jpeg的图片，当然readfile很耗内存，这是最笨的办法

随机返回

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9336046&amp;ptid=757156" target="_blank"><font color="#999999">hjvn2211445 发表于 2020-10-22 14:57</font></a></font><br />
api.diskgirl.com/image/api.php</blockquote></div><br />
这娘们<img src="static/image/smiley/default/loveliness.gif" smilieid="28" border="0" alt="" /><img id="aimg_L266d" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9336046&amp;ptid=757156" target="_blank"><font color="#999999">hjvn2211445 发表于 2020-10-22 14:57</font></a></font><br />
api.diskgirl.com/image/api.php</blockquote></div><br />
求个源码
