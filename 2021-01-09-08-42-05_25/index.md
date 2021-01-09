# cloudflare的野卡证书怎么搞 有没有MJJ了解


如题 最近发现cloudflare给我颁发的证书都是单域名证书，像这样：<br />
<img id="aimg_j4Fft" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/30/7gP86Kcql3ST2yY.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
每添加一个子域名都要颁发一张新的证书，这在证书透明度日志里面都能查的明明白白的，censys里面子域名一览无余，全都暴露出来了，根本没法隐藏...<br />
我知道收费的证书是野卡，而且不是sni.cloudflaressl.com的sni证书，不会被qiang的那种。但有的站用的应该是免费的套餐，但却有野卡的sni证书，像这样：<br />
<img id="aimg_iuf04" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/30/Q2O8DATSVaqF7ph.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
这个应该是免费的sni野卡证书怎么搞？有没有MJJ了解过 先谢过了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<i class="pstatus"> 本帖最后由 iks 于 2020-10-30 19:46 编辑 </i><br />
<br />
用 CNAME 接入就会发单域名证书，以 sni.cloudflaressl.com 为 commomName<br />
以 NS 接入（官方 NS 和 Partner NS 接入均可）就会发通配符证书，仍以 sni.cloudflaressl.com 为 commonName<br />
<br />
<br />
付费（每月10刀），发放 *.example.com 及至多50个下级域名的通配符证书，这个才是所谓防止被墙的证书<br />
<br />
---<br />
补充：<br />
Partner 界面向下拖曳即可看到 NS 接入需要的 NS 记录了<br />
<img id="aimg_UD6fz" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://s1.ax1x.com/2020/10/30/BNeZHU.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><img id="aimg_VKvS0" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

把cname接入改成dns接入

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376598&amp;ptid=760346" target="_blank"><font color="#999999">艾米休艾米休 发表于 2020-10-30 18:46</font></a></font><br />
把cname接入改成dns接入</blockquote></div><br />
大佬 只能用dns接入吗？cname接入cfp+白票的cf pro很香啊 不能用cname接入吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376610&amp;ptid=760346" target="_blank"><font color="#999999">Xiaomage2333 发表于 2020-10-30 18:48</font></a></font><br />
大佬 只能用dns接入吗？cname接入cfp+白票的cf pro很香啊 不能用cname接入吗？</blockquote></div><br />
改了在改回来<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

插眼<img id="aimg_ZJdpI" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376614&amp;ptid=760346" target="_blank"><font color="#999999">艾米休艾米休 发表于 2020-10-30 18:49</font></a></font><br />
改了在改回来</blockquote></div><br />
改回来cf pro套餐就无了<img src="static/image/smiley/default/mad.gif" smilieid="11" border="0" alt="" /> 暂时还是不改了

CF家SNI证书不是免费的吗？野卡证书什么鬼。

他们家证书一直免费的吧...

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376610&amp;ptid=760346" target="_blank"><font color="#999999">Xiaomage2333 发表于 2020-10-30 18:48</font></a></font><br />
大佬 只能用dns接入吗？cname接入cfp+白票的cf pro很香啊 不能用cname接入吗？</blockquote></div><br />
<br />
可以plesk+ns接入的，方法自己琢磨<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" /> 
