# 刚发现wp 多了文件就宝塔插件查杀到了木马~~


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359309&amp;ptid=758991" target="_blank"><font color="#999999">Alicloud 发表于 2020-10-27 14:56</font></a></font><br />
为什么要用windows驱动wordpress？<br />
全盘查杀，改所有密码，检查文件是不是有后门。<br />
 ...</blockquote></div><br />
没有 这个是 liunix 的&nbsp;&nbsp;第一次中招&nbsp; &nbsp;宝塔 似乎那个河马查杀 是 针对单个网站的&nbsp; &nbsp;宝塔有全盘查杀的 插件吗？？

建议使用官网提供的源，密码尽可能复杂，各端口不用的就关闭只开必要的，设置好文件权限。其他建议最好用linux系统的比较好。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359416&amp;ptid=758991" target="_blank"><font color="#999999">胖虎 发表于 2020-10-27 15:14</font></a></font><br />
wp挂马大多是用了不干净的主题或者插件。自己注意就行了没必要专门去杀毒。 ...</blockquote></div><br />
小白想问下，在每个站独立数据库密码的情况下，如果用了不干净的主题，后门漏洞这种会波及到其他数据库吗，或者同个小鸡下的的其他网站？<br />
<br />
<br />
<br />
因为刚玩小鸡小时候，几个站都在一起，当时又用了不知道哪里搞的主题，虽然后来删掉主题了，但现在还是有些担心<img src="static/image/smiley/yct/009.gif" smilieid="44" border="0" alt="" />

<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />绑定，我也想知道，用了不干净主题或者插件，会不会在卸载后，依然在数据库里留下点什么之类

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359479&amp;ptid=758991" target="_blank"><font color="#999999">Dio 发表于 2020-10-27 15:21</font></a></font><br />
小白想问下，在每个站独立数据库密码的情况下，如果用了不干净的主题，后门漏洞这种会波及到其他数据库吗 ...</blockquote></div><br />
一般来说不用，如果是走wp漏洞可能会生成一个管理员权限号，把这个删掉，检查下index文件有没有被篡改过，用新主题测一下没有奇怪的链接就行了。<br />
不过如果是从服务器方面黑进去的就另说了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9360058&amp;ptid=758991" target="_blank"><font color="#999999">胖虎 发表于 2020-10-27 17:01</font></a></font><br />
一般来说不用，如果是走wp漏洞可能会生成一个管理员权限号，把这个删掉，检查下index文件有没有被篡改过 ...</blockquote></div><br />
好的，谢谢大佬
