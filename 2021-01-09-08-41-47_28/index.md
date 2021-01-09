# 求助https://files.photo.gallery/ 目录程序怎么不会生成图片缩略图


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273343&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:04</font></a></font><br />
这个看了&nbsp;&nbsp;依旧不知道怎么样才会生成缓存&nbsp;&nbsp;直接加载原图倒是研究出来了&nbsp;&nbsp;但是那样的话加载太慢了 ...</blockquote></div><br />
需要用到 _files/plugins/tasks.php 插件 生成缓存

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273374&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:09</font></a></font><br />
需要用到 _files/plugins/tasks.php 插件 生成缓存</blockquote></div><br />
大佬 插件哪里下载呢？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273384&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:11</font></a></font><br />
大佬 插件哪里下载呢？</blockquote></div><br />
github

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273392&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:13</font></a></font><br />
github</blockquote></div><br />
大佬可以发个链接吗？搜不到啊

php安装fileinfo和exif扩展完美解决<br />
<br />
话说这个为啥总提示授权&nbsp;&nbsp;有开心版嘛？&nbsp;&nbsp;39刀有点贵

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273404&amp;ptid=752101" target="_blank"><font color="#999999">W4ter 发表于 2020-10-8 21:15</font></a></font><br />
php安装fileinfo和exif扩展完美解决<br />
<br />
话说这个为啥总提示授权&nbsp;&nbsp;有开心版嘛？&nbsp;&nbsp;39刀有点贵 ...</blockquote></div><br />
https://www.hostloc.com/thread-751795-3-1.html<br />
<br />
你看这个帖子。。就可以解决了。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273399&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:14</font></a></font><br />
大佬可以发个链接吗？搜不到啊</blockquote></div><br />
https://github.com/mjau-mjau/files.photo.gallery

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273412&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:16</font></a></font><br />
https://github.com/mjau-mjau/files.photo.gallery</blockquote></div><br />
已经加了 为什么还是不行呢？要运行这个php吗？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273428&amp;ptid=752101" target="_blank"><font color="#999999">xshell 发表于 2020-10-8 21:19</font></a></font><br />
已经加了 为什么还是不行呢？要运行这个php吗？</blockquote></div><br />
<br />
php安装fileinfo和exif扩展完美解决<br />


<i class="pstatus"> 本帖最后由 xshell 于 2020-10-8 21:25 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9273450&amp;ptid=752101" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-8 21:22</font></a></font><br />
php安装fileinfo和exif扩展完美解决</blockquote></div><br />
<br />
安装了啊<br />
<br />
图片处理库<br />
<br />
ImageMagick&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; GD library&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; EXIF&nbsp; &nbsp; &nbsp; &nbsp; Yes<br />
网络通信库<br />
<br />
cURL&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; Sockets&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; Swoole&nbsp; &nbsp; &nbsp; &nbsp; No<br />
文件和字符串处理库<br />
<br />
Ftp&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; bz2&nbsp; &nbsp; &nbsp; &nbsp; No&nbsp; &nbsp; &nbsp; &nbsp; Xmlrpc&nbsp; &nbsp; &nbsp; &nbsp; Yes<br />
Mbstring&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; FileInfo&nbsp; &nbsp; &nbsp; &nbsp; Yes&nbsp; &nbsp; &nbsp; &nbsp; xsl&nbsp; &nbsp; &nbsp; &nbsp; No
