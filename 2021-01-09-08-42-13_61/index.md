# 怎么找到全国IDC机房的IP段？


如题，想查一下网宿的IDC机房IP段，看了下IPIP.NET 还要询价 似乎很贵。<br />
<br />
有什么方法能够看到某个IDC用的IP段吗？<br />
<br />
<br />
<br />
主要用来做CloudFront的CDN国内节点查找，总不能全国IP找一遍吧，印象中AWS国内好像用了网宿的IP段，想直接找网宿的来查，有其他方法的MJJ也来说一下

CloudFront 的 IP 都混在家宽里了，连 ipip.net 也统计不到<br />
另外，网宿的基本半残，建议全网扫<img id="aimg_Kao4C" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380967&amp;ptid=760630" target="_blank"><font color="#999999">iks 发表于 2020-10-31 16:03</font></a></font><br />
CloudFront 的 IP 都混在家宽里了，连 ipip.net 也统计不到<br />
另外，网宿的基本半残，建议全网扫 ...</blockquote></div><br />
真就全网扫啊...&nbsp;&nbsp;太离谱了吧。&nbsp;&nbsp;网宿半残是指的是ws残废吧？&nbsp;&nbsp;拿来做棉被有影响吗？

1. 网宿基本没几个活着的了。<br />
2. 很多节点 ip 藏得很深，而且 ip 的邻居不一定是 cf 节点。<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9380975&amp;ptid=760630" target="_blank"><font color="#999999">Madlifer 发表于 2020-10-31 16:05</font></a></font><br />
真就全网扫啊...&nbsp;&nbsp;太离谱了吧。&nbsp;&nbsp;网宿半残是指的是ws残废吧？&nbsp;&nbsp;拿来做棉被有影响吗？ ...</blockquote></div><br />
您好，有的<br />
建议理解原文，ws残废指的是网宿的节点残废，非 WebSocket 残废<img id="aimg_hO9ZI" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

网宿全部IP段如下<br />
https://drive.google.com/file/d/1z2fEjXoVpsf39dvHxhz2hNCEq5cvXSiE/view?usp=sharing

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381044&amp;ptid=760630" target="_blank"><font color="#999999">xuxu 发表于 2020-10-31 16:22</font></a></font><br />
网宿全部IP段如下<br />
https://drive.google.com/file/d/1z2fEjXoVpsf39dvHxhz2hNCEq5cvXSiE/view?usp=sharing ...</blockquote></div><br />
大佬给个权限<br />


机房的IP段？你想干嘛噢

国内IDC机房和运营商家宽商宽IP混用的，基本不能统计出来
