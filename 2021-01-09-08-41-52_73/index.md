# 腾讯cos套自家cdn，外面再套百度云加速，可以吗？


<i class="pstatus"> 本帖最后由 zhijuefe 于 2020-10-29 10:37 编辑 </i><br />
<br />
用腾讯云cos放了很多文件，由于不想暴露cos地址，于是用 回源鉴权+腾讯自家cdn 来保护cos。<br />
也就是说cos没法直接访问，只能通过腾讯自家的cdn来访问。<br />
<br />
但是腾讯cdn太贵，想再腾讯cdn外面再套百度云加速.&nbsp;&nbsp;百度云加速有代理一年只要600元，每天限量100G。<br />
<br />
这样可行吗？

我觉得可能不太行吧，你自己试试

不要用百度云加速，收费版的不知道，免费的移动流量全没了<img id="aimg_y0d02" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

感觉用的起cos的，应该就会用的起cdn吧。

腾讯云CDN还贵？？？

私有储存桶桶，加个白名单网址防盗链，用网盘程序来限制分享次数<br />
<br />
域名套上CF防止被无限刷分享链接<br />
<br />
这个方案是不是更符合逻辑一点，目前我在用Zpan程序这样干

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367790&amp;ptid=759689" target="_blank"><font color="#999999">Madlifer 发表于 2020-10-29 09:53</font></a></font><br />
私有储存桶桶，加个白名单网址防盗链，用网盘程序来限制分享次数<br />
<br />
域名套上CF防止被无限刷分享链接</blockquote></div><br />
他都上鉴权了，分享不出去的。链接有时效性。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367837&amp;ptid=759689" target="_blank"><font color="#999999">siyi 发表于 2020-10-29 10:01</font></a></font><br />
他都上鉴权了，分享不出去的。链接有时效性。</blockquote></div><br />
分享链接分享的是网盘页面啊,给你看下我的<br />
<br />
<img id="aimg_bVn4k" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/29/ZYPcdvoqM8nSLXQ.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
目前是开了储存桶私有读写、白名单防盗链<br />
<br />
可以正常下载的

确实不知道这操作

理论上 CDN 可以 套 CDN
