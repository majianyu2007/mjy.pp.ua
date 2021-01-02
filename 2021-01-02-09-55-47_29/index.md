# 需要3-5TB的备份，哪个网盘最便宜


阿里云对象存储<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

天翼云盘，便宜又大碗<img id="aimg_sq877" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<img src="static/image/smiley/yct/003.gif" smilieid="50" border="0" alt="" />3.5T可以看看历史贴，或E5E3<br />
付费的百度云应该可以

天翼云盘或者世纪互联吧，不过天翼的好像不能转移了，可惜<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

备份超3年建议自购硬盘

<div class="quote"><blockquote><font color="#999999">insightfy 发表于 2020-10-23 23:48</font><br />
<font color="#999999">我有E3 msdn&nbsp;&nbsp;刚好没人用 楼主需要稳定的存储 同时资料不是限制类的敏感资源可以给你开个子用户 比365稳 ...</font></blockquote></div><br />
我想要

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9344118&amp;ptid=757813" target="_blank"><font color="#999999">lisa1937 发表于 2020-10-24 01:26</font></a></font><br />
目前自用最稳是20+TD盘 rclone自动同步。<br />
有本事20个教育盘同时都掉呀</blockquote></div><br />
有没有如何实现的教程啊，rclone同步需要耗流量不=-=。<br />
有点想学，但网上搜了下，貌似相关教程有点少。

<i class="pstatus"> 本帖最后由 lisa1937 于 2020-10-26 00:56 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9347132&amp;ptid=757813" target="_blank"><font color="#999999">xixi3 发表于 2020-10-24 19:19</font></a></font><br />
有没有如何实现的教程啊，rclone同步需要耗流量不=-=。<br />
有点想学，但网上搜了下，貌似相关教程有点少。 ...</blockquote></div><br />
<br />
vps重启时执行一次同步(gd1 gd2换成你的两个盘)<br />
<br />
nano /etc/crontab<br />
<br /><div class="quote"><blockquote>@reboot root rclone copy --drive-server-side-across-configs --transfers 6 gd1: gd2:&nbsp;&nbsp;&gt;/dev/null 2&gt;&amp;1 &amp;</blockquote></div>

百度网盘一个年付立马就是3T+
