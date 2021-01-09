# 请问大佬们，怎么屏蔽全球机房IP段啊


我发现很多都是通过机房的机器来的。。。<br />
<br />
<br />


0.0.0.0 - 255.255.255.255<br />
<br />
这样就屏蔽掉了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

这方面得请教Netflix

你得自建cdn 自建IP库 买IP数据 做流量清洗 搞网络协议<br />
<br />
<img id="aimg_aUaYc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://imgurl.mxdreamx.com/2020/10/20/TOIMG3555c1020074632N.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 hardwar 于 2020-10-21 23:51 编辑 </i><br />
<br />
<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" />首先拿一份机房IP段列表，然后nginx拉黑（废话<br />
<br />
至于哪里有免费的IP列表，我不知道<img src="static/image/smiley/yct/006.gif" smilieid="32" border="0" alt="" /><br />
<br />
（国外IP基本来自那些知名IDC吧，上 bgp.he.net 找那些ASN下的IP拉起来一波A了。国内不知道

帮顶，来看答案，学习知识的！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

进来学习下

<i class="pstatus"> 本帖最后由 翠花 于 2020-10-21 23:45 编辑 </i><br />
<br />
我也想这样做，但只找到部分：<br /><div class="blockcode"><div id="code_RnO"><ol><li>https://github.com/trick77/ipset-blacklist</ol></div><em onclick="copycode($('code_RnO'));">复制代码</em></div><div class="blockcode"><div id="code_yPS"><ol><li>https://github.com/firehol/blocklist-ipsets</ol></div><em onclick="copycode($('code_yPS'));">复制代码</em></div><div class="blockcode"><div id="code_uu8"><ol><li>https://github.com/XOS/BlockIPs</ol></div><em onclick="copycode($('code_uu8'));">复制代码</em></div><div class="blockcode"><div id="code_Ujj"><ol><li>https://github.com/gaoyifan/china-operator-ip</ol></div><em onclick="copycode($('code_Ujj'));">复制代码</em></div><br />
再结合防火墙开启浏览器验证和人机验证，再把搜索引擎给排除出去。暂时只能先这样了。

海外的还好说，机房基本都有自己的ASN，国内很多IP和家宽都是混在一起的，不仔细筛选根本看不出来。

检测UA，UA不对，一律阻止。
