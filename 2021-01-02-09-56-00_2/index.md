# 哪个dns 解析服务可以强制走https？


<i class="pstatus"> 本帖最后由 总是吵架的猪 于 2020-11-4 19:54 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403269&amp;ptid=762466" target="_blank"><font color="#999999">chunqq 发表于 2020-11-4 19:51</font></a></font><br />
之前搜hsts的时候在csdn看见过</blockquote></div><br />
我搞错了<br />
抱歉<br />
真的有这个啊<br />
<br />
https://zhuanlan.zhihu.com/p/130946490<br />
<br />
预加载名单 硬编码到浏览器

有啥可以利用的？国内主机套cf还不如国外的套 最起码回源是很快的

国内需要北岸的是域名，跟服务器没有关系<br />
<br />
CF的CDN是国外的，本来就不需要北岸域名，当然可以用国内的服务器了<br />
<br />
而要用国内的DNS和CDN域名都需要北岸，你用哪里的服务器跟北岸没有关系。

楼主先分清楚DNS、HTTP、HTTPS这些协议都是做什么的<br />
如果有难度，至少搞清楚他们默认的工作端口&nbsp;&nbsp;<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" />

建议关站回家种地<br />
 哈哈哈

你连 DNS, HTTP 和 HTTPS 都不知道是什么还说得头头是道…哪来的自信…还绕北岸…建议再学下北岸拦截机制

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9403227&amp;ptid=762466" target="_blank"><font color="#999999">keramist 发表于 2020-11-4 19:39</font></a></font><br />
开了cdn 就可以只使用443端口<br />
也是在dns那里设定的规则<br />
cloudflare</blockquote></div><br />
cloudflare也是在80端口做了跳转，没你想得那么高级。

cloudflare只是反代+强制SSL而已 你直接解析到服务器ip 443端口也能访问 80会显示北岸

<i class="pstatus"> 本帖最后由 VULLUV 于 2020-11-4 21:47 编辑 </i><br />
<br />
感觉楼主没有搞清楚cdn、dns等概念<br />
<br />
光靠现在已经普遍使用的dns记录，暂时还无法指定协议

很多人都没懂楼主的意思，未北岸，直接在DNS那边强制跳转到https，不经过服务器80端口跳转，直接在dns跳转
