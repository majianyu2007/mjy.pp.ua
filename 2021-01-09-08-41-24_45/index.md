# 腾讯清凉云对支付宝当面付有debuff？


<i class="pstatus"> 本帖最后由 求道鱼 于 2020-10-25 21:25 编辑 </i><br />
<br />
如题，以前Azure 用的好好的，翻过几次车后，索性买了个香港节点的清凉。<br />
但是据小伙伴反馈，提交订单后，大概要等5-10秒才会返回结果，甚至还有10秒超时现象。<br />
<br />
开始以为是环境问题，结果用宝塔 里面的zfaka 一键部署还是一样，5-10秒。<br />
<br />
换用ion 11.11 测试发现0.3秒！！

两个死对头，延迟对方，也是正常！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> <img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> <img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> 问了支付宝客服，也没支付宝网关的ip 白名单

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351319&amp;ptid=758380" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-25 21:18</font></a></font><br />
两个死对头，延迟对方，也是正常！</blockquote></div><br />
你这样说好像也是那么回事儿<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

清量不清楚，普通的良心云主机用当面付没问题

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351331&amp;ptid=758380" target="_blank"><font color="#999999">Tcpicp 发表于 2020-10-25 21:25</font></a></font><br />
清量不清楚，普通的良心云主机用当面付没问题</blockquote></div><br />
大陆没得问题，不知道是不是hk的原因

不知道哦，这你得检查腾讯的机器和支付宝那边的连通

你拿腾讯/阿里的ip去对ping就知道了<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" />

抓个包 看看就知道了。

我这没事啊，一两秒就可以了
