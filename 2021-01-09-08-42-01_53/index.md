# 在闲置PR上安装了AdGuardHome


<i class="pstatus"> 本帖最后由 寒冰飞雪 于 2020-10-30 09:31 编辑 </i><br />
<br />
主要为软路由上的V2做解析<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />，会不会用一段时间被发现封机器啊<br />
<img id="aimg_jPXz6" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.niupic.com/images/2020/10/29/8VPa.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 88232128 于 2020-10-29 23:29 编辑 </i><br />
<br />
这个不好用，只有windows客户端版本才香<img id="aimg_ivbBA" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9372719&amp;ptid=760039" target="_blank"><font color="#999999">88232128 发表于 2020-10-29 23:27</font></a></font><br />
这个不好用，只有windows客户端版本才香</blockquote></div><br />
我软路由里已经安装了一个了，可能是我架构问题只能过滤国内，所以单独搞个过滤国外的

有作用吗过滤的话<img id="aimg_nFTCg" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

这个是干嘛用的？

windows客户端真是好用

没什么用。撑死无聊看看不同客户端解析量h放到国外机器上，还增加解析时间。

好用不？

我装的ad g+smartdns，但是有两个问题，一个是国nei的vps53端口要北岸，所以需要改为别的端口，国w的端口也建议要改不然就被别人当成免费的dns用，最后日志会写满vps；第二个问题就是延迟高，为了降低dns延迟可以启用本地最近的vps，但这么做的问题在于需要一番设置才能让软路由识别非53端口的dns解析。我现在的方法就是通过近点vps实现dns优化和去广告，本地软路由dns指向vps后自身再起一个koolshare的去广告这样就可以双层去广告又不会消耗本地路由过多计算资源（n1就足够了），测试结果是油管app基本20个视频只能出现一到两次广告，其他的国nei网页还是app基本都没广告了。但是代价就是要开个近地的vps……

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9373458&amp;ptid=760039" target="_blank"><font color="#999999">g6162227 发表于 2020-10-30 09:00</font></a></font><br />
我装的ad g+smartdns，但是有两个问题，一个是国nei的vps53端口要北岸，所以需要改为别的端口，国w的端口 ...</blockquote></div><br />
我这样设置没有你这种问题，国nei都是用的局域网DNS，国wai才用的pr那个，而且连接pr DNS不是我们国nei网络去连接的，是你用作上油管的服务器那台去连接pr的DNS，你要是去ad g后台看你就会看到是哪个IP去连接了，我是分开的，pr上的上游DNS只加了国wai的不加国nei的这样可以防止污染，因为我只要用来解析油管那些
