# 请教大佬怎么让反代镜像站去掉robots.txt


源站含有robots.txt<br />
<br /><div class="quote"><blockquote>User-agent: *<br />
Disallow: /</blockquote></div><br />
<br />
反代镜像站需要去掉robots.txt<br />
或者修改内容

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406101&amp;ptid=762746" target="_blank"><font color="#999999">最美嫦娥颜丹晨 发表于 2020-11-5 12:48</font></a></font><br />
为啥要去掉 直接换成自己的不好吗?<br />
<br />
你都反代镜像了 专门指定一个路径到自己的文件不难吧 ...</blockquote></div><br />
宝塔的反代替换有点毛病<br />
反代是成功,内容替换不成功

return 404　

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406157&amp;ptid=762746" target="_blank"><font color="#999999">最美嫦娥颜丹晨 发表于 2020-11-5 12:59</font></a></font><br />
直接把robots指定路径到自己服务器上</blockquote></div><br />
这个怎么指？？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406157&amp;ptid=762746" target="_blank"><font color="#999999">最美嫦娥颜丹晨 发表于 2020-11-5 12:59</font></a></font><br />
直接把robots指定路径到自己服务器上</blockquote></div><br />
同问,怎么实现?

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9406154&amp;ptid=762746" target="_blank"><font color="#999999">h20 发表于 2020-11-5 12:58</font></a></font><br />
return 404　</blockquote></div><br />
<br />
这个方法比较简单方便,谢谢告知
