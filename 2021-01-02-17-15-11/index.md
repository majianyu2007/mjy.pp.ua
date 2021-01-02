# CloudFlare Worker能转发非标准端口吗


不行。非标不可，IP不可。

返回 fetch 对象应该就可以了，一会我试试<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

我记得不行。如果有ipv6，可以用cf解析后绕一下

技术上是可以的，对CF的请求选择80和443，CF对源站的请求改成非标准端口

https://github.com/xiaoyang-liu-cs/booster.js<br />
<br />
用这个就可以<br />
upstream 和 mobileredirect 直接填你的ip+端口

<i class="pstatus"> 本帖最后由 dole 于 2020-10-14 15:32 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9297101&amp;ptid=753719" target="_blank"><font color="#999999">tkzc 发表于 2020-10-14 08:48</font></a></font><br />
https://github.com/xiaoyang-liu-cs/booster.js<br />
<br />
用这个就可以</blockquote></div><br />
大佬 我这不通<br />
域名：端口Error 1101 Ray ID: 5e1f96f21feea58e • 2020-10-14 07:29:30 UTC<br />
Worker threw exception worker.js:65 Uncaught (in promise) TypeError: Invalid URL string.<br />
&nbsp; &nbsp; at fetchAndApply (worker.js:65)<br />
&nbsp; &nbsp; at worker.js:33<br />
fetchAndApply @ worker.js:65<br />
(anonymous) @ worker.js:33<br />
Promise.catch (async)<br />
(anonymous) @ worker.js:33<br />
Uncaught (in response) TypeError: Invalid URL string.<br />
<br />
ip:端口Error 1003 Ray ID: 5e1f91e2e681f8bb • 2020-10-14 07:26:02 UTC<br />
Direct IP access not allowed<img id="aimg_Rw21G" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

dd<img id="aimg_QhkN3" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

dd<img id="aimg_fLphq" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9299531&amp;ptid=753719" target="_blank"><font color="#999999">dole 发表于 2020-10-14 15:26</font></a></font><br />
大佬 我这不通<br />
域名：端口Error 1101 Ray ID: 5e1f96f21feea58e • 2020-10-14 07:29:30 UTC<br />
Worker threw ...</blockquote></div><br />
网址没输对吧，端口也要在引号里面

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9300766&amp;ptid=753719" target="_blank"><font color="#999999">tkzc 发表于 2020-10-14 19:01</font></a></font><br />
网址没输对吧，端口也要在引号里面</blockquote></div><br />
<br />
我是这样填的<div class="blockcode"><div id="code_fYt"><ol><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;upstream: '42.1.1.1:60906',<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;mobileRedirect: '42.1.1.1:60906' <br /><li>提示不允许ip访问<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;upstream: 'http://42.1.1.1:60906',<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;mobileRedirect: 'http://42.1.1.1:60906'<br /><li>worker错误<br /><li></ol></div><em onclick="copycode($('code_fYt'));">复制代码</em></div><img id="aimg_Yj9NJ" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
