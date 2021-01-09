# Chevereto Free 支持中文命名的图片上传后不变文件名吗？


试了几次，在MySQL 5.5上以及在更高版本支持UTF-8的MariaDB 10.3版本上安装，但如果图片的文件名含有中文，比如“全球主机论坛LOGO.jpg”类似这样的文件命名，则上传后它会自动更改为英文这样的，而不能保持原中文文件名。<br />
<br />
以前我以为是与MySQL对中文的支持有关，后来用了MariaDB 10.3版后，情况依然如此。<br />
<br />
不知安装了这个软件的图床的网友们也是同样的情况吗？

帮顶，没有使用过！<br />
<br />
大佬们回答吧！<br />
<br />
<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9361552&amp;ptid=759179" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-27 22:07</font></a></font><br />
帮顶，没有使用过！<br />
<br />
大佬们回答吧！</blockquote></div><br />
多谢支持，继续等

作者在论坛里，帮你<a href="https://www.hostloc.com/home.php?mod=space&amp;uid=25315" target="_blank">@Chevereto</a> 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363668&amp;ptid=759179" target="_blank"><font color="#999999">Uler 发表于 2020-10-28 01:25</font></a></font><br />
作者在论坛里，帮你@Chevereto</blockquote></div><br />
亲，<br />
<br />
感谢您引起我的注意。<br />
<br />
在V3中，系统使用函数G \ get_filename_by_method（lib/G/functions.php）来生成文件的安全使用的字母数字名称。 这是从V1开始实施的，老实说，我不知道是否仍然需要这样做。 我相信它应该支持文件名中的任何UTF-8字符，我将对此进行调查。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366780&amp;ptid=759179" target="_blank"><font color="#999999">hellfires 发表于 2020-10-28 23:07</font></a></font><br />
我记得自动重命名是可以关的，在设置里，跟中文没关系吧</blockquote></div><br />
<img id="aimg_ehVkV" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/29/BJVn6U.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
我遇到的情况是选择了保留原文件名后，如果是比如英文的或数字的，那么它保留原文件名，但如果原文件名是中文的，如前述例“全球主机论坛.jpg”，那么上传后无法保留原中文名，而会被重新命名。
