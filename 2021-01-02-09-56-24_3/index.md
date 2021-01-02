# 关于网站套cdn之后 无法禁止某些ip访问网站的问题


救救我吧&nbsp;&nbsp;大哥们 我想要安全性和速度和灵活性同时享受

CDN就支持禁用IP;<br />
或者X_FOR传入IP过来你在本地禁用

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451059&amp;ptid=766414" target="_blank"><font color="#999999">xuxu 发表于 2020-11-13 23:14</font></a></font><br />
CDN就支持禁用IP;<br />
或者X_FOR传入IP过来你在本地禁用</blockquote></div><br />
我用的小厂的&nbsp;&nbsp;请问大佬有推荐的好用的cdn吗&nbsp;&nbsp;免北岸的

如果只是CF，是可以在header里面获取到原始IP的，再小厂的CDN都有保留原始IP的，这是基本操作

那就在第一层cdn那里操作啊
