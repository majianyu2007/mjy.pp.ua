# 想問下，軟路由性能


<i class="pstatus"> 本帖最后由 s920361 于 2020-10-28 02:36 编辑 </i><br />
<br />
想問下，考慮組台軟路由。<br />
<br />
2port，一個對外一個對內，速度10Gbps<br />
對內接上L2無網管10Gbps的交換機<br />
<br />
軟體上不做NAT，只做routing<br />
但是軟路由要負責主動入侵防禦和DDoS防禦<br />
<br />
目前考慮使用pfsence+Snorby<br />
<br />
想問下i7 8700或是i9 9900k可以跑滿10Gbps帶寬嗎？<br />
<br />
可以抗得住DDoS嗎？<br />
<br />
================更新==================<br />
<br />
<br />
因為不是花我的錢，幫實驗室弄的，規格就想說開高一點<br />
<br />
實驗室有一個對外10G口，一個class c的公網ip段。<br />
對內應該有100台左右的電腦/NAS/server，還有幾台wifi分享器之類的，給手機/筆電連線<br />
<br />
主要是想在出口網關做一些防掃描/防入侵/防DDoS之類的<br />
有人在掃描裡面電腦的port/ssh爆破，直接在網關ban ip<br />
<br />
因為我自己也不是很有概念，於是想上來請教下大佬<br />
<br />
純粹轉發(我猜)應該夠跑滿10G吧？<br />
但是加上入侵檢測/封包過濾，就不知道性能夠不夠了...

主要的不是流量，而是连接数 包数量。如果全是64K的包i7 pfsense是跑不了10G线速的。大流量如果连接数几十万上百万x86路由得用dpdk之类零拷贝技术才能跑10G线速.<br />


太高端了！<br />
<br />
这种我回答不了！<br />
<br />
我对那啥500M已经满足了！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

没试过这么高的处理器做软路由，楼下大佬解答。

这配置。。。认知盲区<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

没试过10Gbps, 不过8700应该能跑满了。<br />
不过10gbps要注意发热, 还有pfsense是否能支持这个网卡芯片.<br />
<img src="static/image/smiley/default/sweat.gif" smilieid="10" border="0" alt="" />

koolshare有9700k跑万兆，自己搜

话题太高端，我以为n1那种

因為不是花我的錢，幫實驗室弄的，規格就想說開高一點<br />
<br />
實驗室有一個對外10G口，一個class c的公網ip段。<br />
對內應該有100台左右的電腦/NAS/server，還有wifi分享器之類的<br />
<br />
主要是想在出口網關做一些防掃描/防入侵/防DDoS之類的<br />
有人在掃描裡面電腦的port/ssh爆破，直接在網關ban ip<br />
<br />
因為我自己也不是很有概念，於是想上來請教下大佬<br />
<br />
純粹轉發(我猜)應該夠跑滿10G吧？<br />
但是加上入侵檢測/封包過濾，就不知道性能夠不夠了...

没试过这么高端的，但是我觉得跑满10G还是很容易的，但是用户数多的话，不知道能不能抗的住。能不能抗DDoS还得看软件配置了把<br />
<br />
这种建议上硬件防火墙了，感觉是花钱找麻烦<img id="aimg_hsd1v" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
