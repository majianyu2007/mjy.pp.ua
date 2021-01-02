# 被DNS污染或墙了的域名如果我手动设置电脑hosts后 可访问?


比如一个域名是解析的香港IP, 被强了后普通用户就解析不出来真实IP了, 但是我如果手动修改自己电脑hosts把该域名指向真实IP, 是否就可以打开了?<br />
<br />
同理, 如果把google也手动指向成指定IP, 我自己访问可以访问到吗? 

应该不行！有墙！<br />
<br />
<img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" /><img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" /><img src="static/image/smiley/default/smile.gif" smilieid="1" border="0" alt="" />

要是ip没事只是域名dns污染了，本地修改host是可以的。谷歌的ip被杀了，改host无解

DNS污染可以通过修改hosts或者换无污染DNS解决，被墙只能北岸洗白

墙有三种方式，DNS污染、HTTP 阻断和 SNI Reset<br />
墙掉大部分域名的方法都是DNS污染，此时使用hosts是可用的<br />
17年以后墙启用了SNI Reset，即审查TLS证书，若包含黑名单域名则阻断链接，目前仅对大站（Google, FB, 推特 等）启用，所以你的不知名的域名被污染了可以指定hosts，但对Google不行<img id="aimg_A6B3G" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

103.91.210.120 www.google.com<br />
<br />
设置上面那个后, 我刚才访问确实打开了

话说现在上https的站&nbsp;&nbsp;移动好像也能屏蔽了

墙是80&nbsp;&nbsp;污染是DNS级。。。所以区分开来的话 相对能细致的针对性进行。。。抢救。。。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449612&amp;ptid=766317" target="_blank"><font color="#999999">iks 发表于 2020-11-13 17:56</font></a></font><br />
墙有三种方式，DNS污染、HTTP 阻断和 SNI Reset<br />
墙掉大部分域名的方法都是DNS污染，此时使用hosts是可用的<br />
 ...</blockquote></div><br />
<br />
长见识了，怪不得之前用过修改DNS富强，没过多久就不行了。
