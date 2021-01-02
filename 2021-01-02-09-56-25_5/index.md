# mac升级big sur之后苹果应用商店的wireguard组内网无法上网


昨天心血来潮把mac升级到最新的big sur了，结果一晚上升级早上起来看了下，发现浏览器都没法上网了，排查了很久才发现是wireguard的问题，断开就一切正常，连上wireguard就ping不通任何域名，但是wireguard组的内网都是通的，就是意味着扶墙的服务器端是能连上的，后来试了一下，发现用ip访问的网站都正常能打开，所以排除了网络不通的问题。<br />
<br />
从现象看应该就是dns解析有问题，不知道wireguard客户端到底干了啥，不过我去app store上面看了下，也是一年前更新的，很久没更新了。<br />
<br />
后来试了下用brew安装了下wireguard，直接通过命令行，使用原先客户端使用的配置文件，发现一切都正常。能正常上网，能正常访问wireguard内网。<br />
<br />
每次mac更新都要给我整点事情出来。<br />
<br />
上次升级到上一个版本到时候，btsync用不了了，搞了个docker跑linux版本，效果都不太好，现在都还郁闷中，这次差点搞的上不了网，哎

我早也更新了，目前发现一个小问题。sublime text 3 使用 source code pro 字体的时候，代码不着色。<br />
换回默认字体解决。

还可以

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9452944&amp;ptid=766596" target="_blank"><font color="#999999">小夜 发表于 2020-11-14 13:36</font></a></font><br />
我早也更新了，目前发现一个小问题。sublime text 3 使用 source code pro 字体的时候，代码不着色。<br />
换回 ...</blockquote></div><br />
大佬知道sublime text老是弹出更新提升怎么办吗？烦死了<br />
<br />
<img id="aimg_L0elb" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://www.jiasuzhu.com/images/2020/11/14/2020-11-14-1.50.58.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9452944&amp;ptid=766596" target="_blank"><font color="#999999">小夜 发表于 2020-11-14 13:36</font></a></font><br />
我早也更新了，目前发现一个小问题。sublime text 3 使用 source code pro 字体的时候，代码不着色。<br />
换回 ...</blockquote></div><br />
我都不知道我用的啥字体··

15年的老机器坚决不升级

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9453017&amp;ptid=766596" target="_blank"><font color="#999999">forever8938 发表于 2020-11-14 13:53</font></a></font><br />
15年的老机器坚决不升级</blockquote></div><br />
我就是15年的air&nbsp;&nbsp;手痒给升级了

你号没了
