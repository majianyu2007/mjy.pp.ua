# 宝塔一键搬迁inode满了，求清理命令


搬了几个网站就提示失败了，宝塔技术说 inode满了，叫我删除，又不告诉我怎么弄，我是菜鸟。<br />
<br />
<br />
百度只查到这2条命令<br />
<br />
df -i<br />
<img id="aimg_ej3ve" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/28/B1JpMq.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
cd /<br />
du -sh *<br />
<br />
<img id="aimg_XLWcz" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/28/B1JIkF.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
求懂LINUX的高手给条删除命令<br />
<br />
<font color="Red">rm -f ./*</font><br />
<br />
这个命令我试过，数据全没了，别给我出损招 谢谢了。

rm -rf ./*<br />
多试几次，肯定能成功

不会&nbsp;&nbsp;给你顶上去

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363055&amp;ptid=759319" target="_blank"><font color="#999999">cherbim 发表于 2020-10-28 11:06</font></a></font><br />
rm -rf ./*<br />
多试几次，肯定能成功</blockquote></div><br />
要是小白真的在生产环境上面用了你这个命令就真的完蛋了，希望不要开这种玩笑。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363072&amp;ptid=759319" target="_blank"><font color="#999999">yanaxiao 发表于 2020-10-28 11:10</font></a></font><br />
要是小白真的在生产环境上面用了你这个命令就真的完蛋了，希望不要开这种玩笑。 ...</blockquote></div><br />
严重同意<br />
很多小白都不知道这个是干什么的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363072&amp;ptid=759319" target="_blank"><font color="#999999">yanaxiao 发表于 2020-10-28 11:10</font></a></font><br />
要是小白真的在生产环境上面用了你这个命令就真的完蛋了，希望不要开这种玩笑。 ...</blockquote></div><br />
<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" /><br />
我之前就看见过一个真实直播，一个小站长真的一路yes下去了<img id="aimg_Cjpq5" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

楼上其实没错，你进到那个小文件目录执行这个<br />
可能他没说清楚，这个一般就是删，或者扩容了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363080&amp;ptid=759319" target="_blank"><font color="#999999">GAted0 发表于 2020-10-28 11:12</font></a></font><br />
我之前就看见过一个真实直播，一个小站长真的一路yes下去了</blockquote></div><br />
要是在测试环境，或者不重要的机子上还好说，真的在生产机上执行了，那估计只能跑路了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363087&amp;ptid=759319" target="_blank"><font color="#999999">yanaxiao 发表于 2020-10-28 11:14</font></a></font><br />
要是在测试环境，或者不重要的机子上还好说，真的在生产机上执行了，那估计只能跑路了。 ...</blockquote></div><br />
真的，那个站长跑路了。。做的资源素材站，后来还退群了，估计也没备份<img id="aimg_trjoA" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

挂载 GD
