# 端口能Ping通的情况下，为什么协议无法 正常连接？


<i class="pstatus"> 本帖最后由 cgcg 于 2020-10-23 13:23 编辑 </i><br />
<br />
目前我购买的主机，自定义的8080端口可以ping通，主机也重装系统和Snell协议了，但是无法 正常使用。<br />
<br />
同样的操作在其他境外主机上正常。也尝试切换了本地电信及移动的网络，均无法连接。<br />
<br />
老铁们来帮忙看看

常见的代理是基于tcp协议的。<br />
应该测试tcping的情况。<br />
ping是icmp协议的，不一样。<br />
tcping不正常，ping 正常没用。<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
建议去了解xxx阻断
