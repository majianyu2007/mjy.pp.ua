# aria2 如何通过https连接？


aria2 通过http可以连接上，通过https老是连不上。已经通过docker部署了ariaNG，也通过nginx反代能正常加载网页了，但是就是死活连不上，请问啥原因？

我觉得你没把问题说清楚， 是aria2的web客户端无法链接aria2 api么&nbsp;&nbsp;<br />
应该是api配置的原因， 第一点aria2 api的https你准备在aria2里配置还是在nginx里面配置， 第二点 注意js api跨域问题

aria2配置文件里面rpc的地址的证书目录和https开关填了没

楼上说的对，配置文件里也要改

https://cloud.tencent.com/developer/article/1544695 按照此贴的说法，已经在aria2配置文件里面添加了允许https连接，而且添加了证书和key，但是还是不行

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9336402&amp;ptid=757190" target="_blank"><font color="#999999">Lison 发表于 2020-10-22 16:03</font></a></font><br />
aria2配置文件里面rpc的地址的证书目录和https开关填了没</blockquote></div><br />
用这个镜像jwilder/nginx-proxy 反代的，请问证书目录应该是rpc-certificate=/opt/proxy/proxy/certs/域名.crt和rpc-private-key=/opt/proxy/proxy/certs/域名.key 吧（就是certs目录下面的这两个文件？）

Nginx反代为什么aria2配置还要配置https?Nginx配置成https，proxy_pass到RPC端口。连接页面: 域名:443/jsonrpc

AriaNg和Aria2都不使用https不就行了，一个下载工具弄这么复杂干嘛？

修改 aria2 的配置，<br />
<br />
开启证书，指定证书目录<br />
<br />
重启ara2<br />
<br />
就Ok了

在nginx配置好https反代到aria2和ariaNg 然后配置里<br />
<a href="https://www.hostloc.com/" target="_blank">http s://aria2.demo.com:443</a> 密钥就行了jsonrpc<br />
因为我就是用docker方式布署好nginx aria2 ariaNg也是用https来访问
