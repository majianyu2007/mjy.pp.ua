# 认真求解：做站选国内还是国外主机？


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365712&amp;ptid=759220" target="_blank"><font color="#999999">某猫猫 发表于 2020-10-28 19:10</font></a></font><br />
差不多吧,单纯iptables反代也有提升,当然railgun更好<br />
国内腾讯到cf回源点太烂了 ...</blockquote></div><br />
谢谢大佬， 请求一份相关的教程资源， 关键词搜到的都是反代国外是先免北岸的博客，原理好像有一定的不同。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9365932&amp;ptid=759220" target="_blank"><font color="#999999">1aughing 发表于 2020-10-28 20:04</font></a></font><br />
谢谢大佬， 请求一份相关的教程资源， 关键词搜到的都是反代国外是先免北岸的博客，原理好像有一定的不同 ...</blockquote></div><br />
唔,railgun要cf partner,plesk的也行,只要商家愿意帮你配置<br />
不用railgun用iptables的话搜iptables中转<br />
80/443想要复用的话caddy或者sniproxy<br />
源站记得开realip,中转不用管realip也不要写x_forward_for,源站拿cf提供的即可<br />
中转没必要缓存任何东西,缓存只在cdn做

lz看看签名的JJ，做站速度很不错的。而且有DDOS防御。

买个香港的就行 也不用套cdn

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366181&amp;ptid=759220" target="_blank"><font color="#999999">某猫猫 发表于 2020-10-28 20:59</font></a></font><br />
唔,railgun要cf partner,plesk的也行,只要商家愿意帮你配置<br />
不用railgun用iptables的话搜iptables中转<br />
80 ...</blockquote></div><br />
谢谢指导！我先查查看解决的难易度，再来反馈。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366210&amp;ptid=759220" target="_blank"><font color="#999999">秋上书 发表于 2020-10-28 21:02</font></a></font><br />
买个香港的就行 也不用套cdn</blockquote></div><br />
香港也在考虑中； 国内可北岸的情况下，有好的教程嘛？ 

目前一台腾讯云国内套腾讯云全站加速，另一台服务器在法国也是套腾讯云全站加速，有很多站不适合套CDN，但全站加速没有问题<img id="aimg_XUWa5" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363576&amp;ptid=759220" target="_blank"><font color="#999999">1aughing 发表于 2020-10-28 13:02</font></a></font><br />
大佬的是用的香港良心云作站吗？</blockquote></div><br />
小商家，现在已经不用了，就不发了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9366721&amp;ptid=759220" target="_blank"><font color="#999999">1aughing 发表于 2020-10-28 22:52</font></a></font><br />
香港也在考虑中； 国内可北岸的情况下，有好的教程嘛？</blockquote></div><br />
想北岸的话 那现在就是腾讯云的活动了吧 2H4G3M 三年才698 新注册的QQ号认证一下 就是新用户 可以直接买 一个身份证能认证三个号 都能当新用户

CF就别用了，境内使用基本等于自残。
