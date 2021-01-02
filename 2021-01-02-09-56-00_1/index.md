# 哪个dns 解析服务可以强制走https？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403218&amp;ptid=762466" target="_blank"><font color="#999999">sunpma 发表于 2020-11-4 19:37</font></a></font><br />
DNS还能指定HTTPS吗？没听说过啊~~</blockquote></div><br />
开了cdn 就可以只使用443端口<br />
也是在dns那里设定的规则<br />
cloudflare

找個可以設定if port==80 return 301的cdn唄，cf是其中一個<br />
<br />
不要cdn就自己改nginx的規則唄<br />
大概長這樣，大意是如果是80port，就跳轉https<br /><div class="blockcode"><div id="code_Iad"><ol><li>server {<br /><li>&nbsp; &nbsp; listen 80 default_server;<br /><li>&nbsp; &nbsp; server_name _;<br /><li>&nbsp; &nbsp; return 301 https://$host$request_uri;<br /><li>}</ol></div><em onclick="copycode($('code_Iad'));">复制代码</em></div><br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403234&amp;ptid=762466" target="_blank"><font color="#999999">s920361 发表于 2020-11-4 19:42</font></a></font><br />
找個可以設定if port==80 return 301的cdn唄，cf是其中一個<br />
<br />
不要cdn就自己改nginx的規則唄</blockquote></div><br />
服务器上都说了不能80跳转 跳转就是未北岸<br />
<br />
直邮cdn/dns上做文章

什么鬼问题，开启cdn解析就切到cf的节点了，我猜你用的是免费的cf，节点都是海外

HSTS我记得有个谷歌的东西，开一个参数可以把域名提交到谷歌这玩意，然后下次谷歌等主流浏览器更新的时候会把这个域名直接写到chrome等浏览器安装包里，访问的时候直接本地强制https，缺点就是如果以后不用https，这些浏览器就没法访问这个域名；得等下次这些浏览器更新改写进去的域名

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403202&amp;ptid=762466" target="_blank"><font color="#999999">keramist 发表于 2020-11-4 19:33</font></a></font><br />
搞清楚我的问题先 </blockquote></div><br />
建议关站回家种地

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403247&amp;ptid=762466" target="_blank"><font color="#999999">streamer 发表于 2020-11-4 19:45</font></a></font><br />
什么鬼问题，开启cdn解析就切到cf的节点了，我猜你用的是免费的cf，节点都是海外 ...</blockquote></div><br />
<br />
没明白问题？<br />
国外dns/cdn 强制走443 就能使用国内未北岸的服务器<br />
如果先访问80在跳转443 就是提示未北岸<br />
明白了吧？

<i class="pstatus"> 本帖最后由 总是吵架的猪 于 2020-11-4 19:55 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403254&amp;ptid=762466" target="_blank"><font color="#999999">chunqq 发表于 2020-11-4 19:46</font></a></font><br />
HSTS我记得有个谷歌的东西，开一个参数可以把域名提交到谷歌这玩意，然后下次谷歌等主流浏览器更新的时候会 ...</blockquote></div><br />
<br />
 竟然是真的有这个<br />
<br />
我搞错了 抱歉

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403257&amp;ptid=762466" target="_blank"><font color="#999999">宣传 发表于 2020-11-4 19:46</font></a></font><br />
建议关站回家种地</blockquote></div><br />
本来就没开 测试如何利用未北岸服务器而已<br />
回家种地 总比你摇尾乞怜好

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403260&amp;ptid=762466" target="_blank"><font color="#999999">总是吵架的猪 发表于 2020-11-4 19:47</font></a></font><br />
这是你自己想出来的吧<br />
浏览器怎么会捆绑这些东西呢</blockquote></div><br />
之前搜hsts的时候在csdn看见过<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
