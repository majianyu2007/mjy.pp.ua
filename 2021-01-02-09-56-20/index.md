# 大佬们，U盘突然不能制作启动盘了，啥情况


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449340&amp;ptid=766298" target="_blank"><font color="#999999">Nothing1024 发表于 2020-11-13 17:06</font></a></font><br />
用工具重新做或者格式化成FAT32，自己导入引导文件</blockquote></div><br />
格式化为fat32做过，自己导入引导文件？什么引导文件？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449359&amp;ptid=766298" target="_blank"><font color="#999999">michelleman 发表于 2020-11-13 17:09</font></a></font><br />
格式化为fat32做过，自己导入引导文件？什么引导文件？</blockquote></div><br />
PE引导文件，或者系统镜像安装工具的引导文件<br />
或者自己下个grub拷进去看看能不能读出来

不能启动的话，报什么错误？

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9449429&amp;ptid=766298" target="_blank"><font color="#999999">dajiahao 发表于 2020-11-13 17:24</font></a></font><br />
不能启动的话，报什么错误？</blockquote></div><br />
没错误，就是烧录以后启动菜单不显示我的U盘，其他U盘都能正常显示出来

重置一下才行<br />
估计是里面有引导分区或者其他奇奇怪怪的东西

爱国者就是辣鸡，8层是爱国者U盘出现问题了<br />
<br />
建议申请售后或者退款换闪迪吧

格式不一样&nbsp;&nbsp;格式化, 重新做要么,win10不是官方自动制作的么,&nbsp;&nbsp;第三方不敢用

我来给你详细解释下吧，首先要确定有没有回收空间，优启通有回收空间的功能，可以插上去试试，直接格式化会造成不可挽回的错误，比如U盘直接读取不了。<br />
如果要安装Linux系统，需要FAT32格式，而之前的分区格式应该是NTFS，所以如果U盘上面那个方法不行就改分区格式试试，最后，不推荐你用优启通，有那么多好的工具可以用，给你推荐几个，比如usbos，我非常极力推荐，你可能不知道优启通的原作者就是usbos的同一个作者，他后来还是继续选择更新自己的原来作品，退出了优启通的团队，优启通自从商业化后就做的很差，这点我很不喜欢，另外再推荐几个：rufus、balenaetcher、yumi、ventoy等等太多了

磁盘开头的数据区域应该是坏掉了

用微PE最后一种方法制作U盘启动盘（归还空间&amp;合并隐藏分区）<img id="aimg_BJ1oy" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
