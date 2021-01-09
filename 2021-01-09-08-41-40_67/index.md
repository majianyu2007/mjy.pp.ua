# 想問下，軟路由性能


<i class="pstatus"> 本帖最后由 s920361 于 2020-10-28 03:02 编辑 </i><br />
<br />
當初有和廠商談，是我覺得硬件防火牆太貴了，好像一年要10w人民幣/50w台幣左右(因為裡面的軟體也會不斷更新，所以是收年費的)<br />
<br />
所以我和老師毛遂自薦，可以用開源方案自己兜，自己更新軟體，只要一次性費用1w左右就好。<br />
我想說一萬組軟路由，可以組很頂規的吧?<br />
<br />
現在覺得真的是挖坑給自己跳呀...<br />
<br />
順帶問下，「全是64K的包」是什麼意思呀？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9362169&amp;ptid=759192" target="_blank"><font color="#999999">s920361 发表于 2020-10-28 02:58</font></a></font><br />
當初有和廠商談，是我覺得硬件防火牆太貴了，好像一年要10w人民幣/50w台幣左右(因為裡面的軟體也會不斷更新 ...</blockquote></div><br />
64K包应该指的是包转发能力把，软路由这点是不行的，貌似是因为没有硬件加速<img id="aimg_sffW3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 akw28888 于 2020-10-28 05:30 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9362169&amp;ptid=759192" target="_blank"><font color="#999999">s920361 发表于 2020-10-28 02:58</font></a></font><br />
當初有和廠商談，是我覺得硬件防火牆太貴了，好像一年要10w人民幣/50w台幣左右(因為裡面的軟體也會不斷更新 ...</blockquote></div><br />
<br />
他指的應該是 64byte 的 packet<br />
基本上不用指望pfsense... 遇到DDOS是根本撐不住<br />
BSD 的 firewall 也沒有強到可以處理 10Gbps line-rate<br />
<br />
我是覺得Anti-DDoS這一點可以直接當成沒有<br />
真正DDOS打TANET, 什麼設備都沒用~ 隨便DDOS都超過10G.

完全超出思维想象

楼猪联系我， 5K RMB&nbsp;&nbsp;可以跑满12M pps 以上. 64字节小包.<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

性能看需求
