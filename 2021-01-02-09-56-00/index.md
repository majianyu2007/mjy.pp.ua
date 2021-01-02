# 哪个dns 解析服务可以强制走https？


<i class="pstatus"> 本帖最后由 keramist 于 2020-11-4 19:41 编辑 </i><br />
<br />
实测 cloudflare 开启cdn可以强制用https 腾讯不会提示未北岸<br />
只用dns做解析 会提示dns未北岸<br />
<br />
设置规则跳转位https/强制使用https<br />
<br />
有大佬带着一起玩么<br />
<br />
<br />
<br />
必须在dns端就是https 才能正常使用国内未北岸服务器<br />
<br />
服务器上80跳转到443 <br />
就会提示未北岸<br />
<br />
搞清楚问题所在<br />
<br />
<br />
所以国内吃灰的机器 套了国外cdn <br />
比如cloudflre 是可以正常使用的<br />
大家可以利用起来<br />


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403202&amp;ptid=762466" target="_blank"><font color="#999999">keramist 发表于 2020-11-4 19:33</font></a></font><br />
搞清楚我的问题先 </blockquote></div><br />
建议关站回家种地

https 什么时候属于DNS解析的业务范围了 神奇的问题

建议关站回家种地<br />
 哈哈哈

楼主先分清楚DNS、HTTP、HTTPS这些协议都是做什么的<br />
如果有难度，至少搞清楚他们默认的工作端口&nbsp;&nbsp;<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403257&amp;ptid=762466" target="_blank"><font color="#999999">宣传 发表于 2020-11-4 19:46</font></a></font><br />
建议关站回家种地</blockquote></div><br />
本来就没开 测试如何利用未北岸服务器而已<br />
回家种地 总比你摇尾乞怜好

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403218&amp;ptid=762466" target="_blank"><font color="#999999">sunpma 发表于 2020-11-4 19:37</font></a></font><br />
DNS还能指定HTTPS吗？没听说过啊~~</blockquote></div><br />
开了cdn 就可以只使用443端口<br />
也是在dns那里设定的规则<br />
cloudflare

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403177&amp;ptid=762466" target="_blank"><font color="#999999">宣传 发表于 2020-11-4 19:27</font></a></font><br />
hstspreload.org<br />
HSTS preload list了解一下</blockquote></div><br />
搞清楚我的问题先 <br />
<br />
<br />
必须在dns端就变为https<br />
否则访问国内未北岸80端口 不会跳转https 直接变成提示未北岸

什么鬼问题，开启cdn解析就切到cf的节点了，我猜你用的是免费的cf，节点都是海外

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403174&amp;ptid=762466" target="_blank"><font color="#999999">llmwxt 发表于 2020-11-4 19:26</font></a></font><br />
帮顶，我只知道，宝塔可以设置强制HTTPS</blockquote></div><br />
有毛用 <br />
必须在dns端就变为https<br />
否则访问未北岸80端口 不会跳转https <br />
直接变成提示未北岸<br />
<br />
<br />


<i class="pstatus"> 本帖最后由 s920361 于 2020-11-4 19:38 编辑 </i><br />
<br />
我想沒有一家dns可以做到。<br />
<br />
因為dns唯一的用途就是你問他網址，他回答你ip。<br />
<br />
你得要自己設定301轉址，不然就是用別人的server，幫你301轉址<br />
<br />
cf也不過是幫你反代然後301

帮顶，我只知道，宝塔可以设置强制HTTPS<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

hstspreload.org<br />
HSTS preload list了解一下

投资吧 找大厂搞一下

DNS还能指定HTTPS吗？没听说过啊~~

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403213&amp;ptid=762466" target="_blank"><font color="#999999">s920361 发表于 2020-11-4 19:36</font></a></font><br />
我想沒有一家dns可以做到。因為dns唯一的用途就是你問他網址，他回答你ip。你得要自己301轉址 ...</blockquote></div><br />
但是开了cdn就可以做到 使用国内未北岸的服务器 443端口 提供正常服务 <br />
哈哈<br />
所有有啥思路可以利用利用？<br />

