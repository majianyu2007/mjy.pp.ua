# aria2 如何通过https连接？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9336529&amp;ptid=757190" target="_blank"><font color="#999999">osqi 发表于 2020-10-22 16:29</font></a></font><br />
在nginx配置好https反代到aria2和ariaNg 然后配置里<br />
http s://aria2.demo.com:443 密钥就行了jsonrpc<br />
因为 ...</blockquote></div><br />
请问你用的是哪个镜像？

反代6800 源站不需要配置证书，端口443

搞定，原来是证书路径搞错了。谢谢楼上诸位。哇哈哈。

配置里面加上ssl的证书位置
