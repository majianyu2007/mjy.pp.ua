# 请教一下外网访问内外提取数据的问题？


还是我腾讯的小鸡IP被封了，不给开外网访问，我被封机器装的宝塔，现在数据提不出来，我又开了台同一个区的小鸡是在同一个内网，我可否通过这个可以访问外网的机器访问同一内网下被封的小鸡！我只想把数据提出来！研究一上午没搞成，有大佬指导一下不?

<i class="pstatus"> 本帖最后由 xlouspeng 于 2020-10-29 13:19 编辑 </i><br />
<br />
只要两台机器可以通过内网ssh，就可以把数据下载回来<br />
ssh代理即可完美访问文件数据

在控制台操作，<br />
原服务器-制作镜像<br />
新服务器-重装系统-选择制作的那个镜像 <br />
网站和数据就到新服务器上了<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368810&amp;ptid=759773" target="_blank"><font color="#999999">robot 发表于 2020-10-29 13:02</font></a></font><br />
在控制台操作，<br />
原服务器-制作镜像<br />
新服务器-重装系统-选择制作的那个镜像 </blockquote></div><br />
腾讯轻量不能制作镜像！只有快照。又没用！<img id="aimg_lu6f5" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

是可以通过内网机访问被封小鸡的，你也可以找客服解封，你就说你要提数据。我有台腾讯机子被肉鸡也被封IP，找的客服解封的。
