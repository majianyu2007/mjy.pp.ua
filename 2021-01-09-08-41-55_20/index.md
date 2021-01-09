# Frp内网各端口正常但是穿透无法启动（补图）


<i class="pstatus"> 本帖最后由 xxwzdc 于 2020-10-29 15:57 编辑 </i><br />
<br />
如题：最近一直研究Frp穿透，看了很多教程，有两个问题始终无法解决，请教大家一下。一个是服务端严格按照教程操作的，也提示成功启动，端口监听了。VPS的防火墙放行了，系统内部防火墙也停止了。就是无法连接，最简单的frp仪表盘ip+7500端口都打不开。阿里 GCP，甲骨文都试验过了。<br />
第二个问题是 客户端无法启动，也是按照教程配置的，执行客户端启动命令后就是 超时.... .....。全部端口也放行了。哪位大佬指点一下？从哪里入手，都快折腾吐了。<br />
<br />


配置文件呢，

frp服务端启动后，扫描下端口是否开放了。

贴配置文件出来看看

已经补图了<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

<i class="pstatus"> 本帖最后由 tsubasa 于 2020-10-29 16:03 编辑 </i><br />
<br />
<img id="aimg_cdiwG" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/29/BGTVu4.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
不好意思，你远程服务器的7500 7550 7700端口并不通<img id="aimg_FVzRz" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

配置文件用utf8编码

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9369646&amp;ptid=759802" target="_blank"><font color="#999999">tsubasa 发表于 2020-10-29 16:01</font></a></font><br />
不好意思，你远程服务器的7500 7550 7700端口并不通</blockquote></div><br />
我在vps把所有的端口入口都放开了，换了甲骨文 和GCP同样的问题，没有安装宝塔什么的

<i class="pstatus"> 本帖最后由 nisekoi 于 2020-10-29 16:10 编辑 </i><br />
<br />
图片太模糊了。看不清描述的字。不过这种情况大概率就是防火墙没开。系统的，服务商的。软件的。都检查一下

直接 nc -lk -p 12345 监听。然后tcping看端口开没开
