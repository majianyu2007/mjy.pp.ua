# V屁恩连接内网与WIFI局域网IP冲突问题


<i class="pstatus"> 本帖最后由 xixi3 于 2020-10-26 21:31 编辑 </i><br />
<br />
因为NAS部署HTTPS麻烦（存在中间人的风险），而且最近暴露于公网的TR后台一天到晚被人试密码，迫于无奈，决定采用扶墙回内网的方式远程管理NAS。<br />
当我设置好了open扶墙后，通过4G访问一切正常，<strong>通过其他WIFI也成功连接上了扶墙，但当我输入我的内网地址时发现，我的内网IP和它的内网IP是一个网段的，有很多冲突，打不开我的内网设备。</strong><br />
我想到的办法有：1.改变自己的内网网段&nbsp; &nbsp; 2.换个Wifi<br />
MJJ们还有什么其他妙招不？<br />
V屁N被自动替换了，淦，扶墙=V屁N

帮顶，我不知道！<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

没玩过NAS，不知道，帮顶了

open可以设置内网网段的啊

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9356121&amp;ptid=758744" target="_blank"><font color="#999999">sqliuchang 发表于 2020-10-26 21:33</font></a></font><br />
open可以设置内网网段的啊</blockquote></div><br />
主要我OPEN的内网网段和我的设备也不在一个网段，但是NAS自带的虚拟路由功能进行了一个三层交换机的作用。

改个内网网段就行了，又不是定死的<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font color="#999999">xixi3 发表于 2020-10-26 21:35</font><br />
<font color="#999999">主要我OPEN的内网网段和我的设备也不在一个网段，但是NAS自带的虚拟路由功能进行了一个三层交换机的作用 ...</font></blockquote></div><br />
我是开了一个低加密的xxr而不是open

内网网段一定要固定，微屁恩一定也可以设置网段，但我还是建议你的nas还是固定网段较好

二层桥接过去不就行了？关闭某软件的三层交换机

规则，全局。
