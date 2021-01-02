# 请教大家一个旁路由设置的问题


看我的<br />
config interface 'lan'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option ifname 'eth0'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option proto 'static'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option netmask '255.255.255.0'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option ip6assign '60'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option ipaddr '192.168.100.9'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option gateway '192.168.100.1'<br />
&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;option dns '127.0.0.1'

非常感谢楼上几位大佬的热心回复，我就不一一回复了，再次表示感谢，爱你们<img src="static/image/smiley/yct/017.gif" smilieid="40" border="0" alt="" />

1、你路由器的内网IP，你电脑IP，你都没发出。<br />
2、你修改N1的IP，把手动指定改为自动获取呢<br />
三方只知道一方IP，没法测试

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404776&amp;ptid=762552" target="_blank"><font color="#999999">蜗牛也是牛 发表于 2020-11-5 08:25</font></a></font><br />
1、你路由器的内网IP，你电脑IP，你都没发出。<br />
2、你修改N1的IP，把手动指定改为自动获取呢<br />
三方只知道一方 ...</blockquote></div><br />
啊不好意思我补充一下，我路由器的ip是192.168.0.2这个我发过了。电脑ip是192.168.0.101，现在问题是N1后台进不去。。。N1ip是192.168.0.102

你需要手动设置电脑ip为opwenwrt的网段才行，你现在电脑分配的ip是上级路由的<br />

