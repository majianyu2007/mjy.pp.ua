# EHEH.ORG 新增CN2线路检测


<div class="quote"><blockquote><font color="#999999">Eric.c 发表于 2020-10-30 21:58</font><br />
<font color="#999999">不是很明白，来个指点</font></blockquote></div><br />
出海线路如果只走59.43就是gia如果走了59.43又走了202开头的ip就是gt 

已安装，挺有意思，就不知道安全性如何

<div class="quote"><blockquote><font color="#999999">telnetpig 发表于 2020-10-30 23:11</font><br />
<font color="#999999">已安装，挺有意思，就不知道安全性如何</font></blockquote></div><br />
放心放心，监控端代码都是开源的，不会有敏感数据上传哦

我去， ipv6的？<br />
C:\Users\neo&gt;nslookup eheh.org<br />
服务器:&nbsp;&nbsp;OpenWrt.lan<br />
Address:&nbsp;&nbsp;192.168.1.1<br />
<br />
名称:&nbsp; &nbsp; eheh.org<br />
Addresses:&nbsp;&nbsp;2606:4700:20::681a:5b7<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 2606:4700:20::681a:4b7

瓦工DC6 DC9识别成普通线路

<div class="quote"><blockquote><font color="#999999">h1xy 发表于 2020-10-31 02:21</font><br />
<font color="#999999">我去， ipv6的？<br />
C:%users\neo&gt;nslookup eheh.org<br />
服务器:&nbsp;&nbsp;OpenWrt.lan<br />
</font></blockquote></div><br />
v4也有

<div class="quote"><blockquote><font color="#999999">yuanyuexiaoni 发表于 2020-10-31 03:30</font><br />
<font color="#999999">瓦工DC6 DC9识别成普通线路</font></blockquote></div><br />
对，周末改下规则，换个机房

用上了，挺方便，支持

代码跟nodequery一模一样，&nbsp;&nbsp;问下nodequery提交的base64 怎么解密啊

<div class="quote"><blockquote><font color="#999999">cnly1987 发表于 2020-10-31 07:33</font><br />
<font color="#999999">代码跟nodequery一模一样，&nbsp;&nbsp;问下nodequery提交的base64 怎么解密啊</font></blockquote></div><br />
看一下我的脚本顶部说明，这个版本就是基于它改进的。下个大版本会是golang写的
