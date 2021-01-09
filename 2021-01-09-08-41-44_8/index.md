# 宝塔一键搬迁inode满了，求清理命令


楼主还没搞好？<br />
find /tmp -type f -exec rm {} \;<br />
find /home -type f -size 0 -exec rm {} \;<br />
运行后，还不行，再来找我

一个个都想要小白rm 。。。<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

给出rm命令的都是坑爹玩意

删除你的静态小文件就可以

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9363378&amp;ptid=759319" target="_blank"><font color="#999999">lanying 发表于 2020-10-28 12:13</font></a></font><br />
删除你的静态小文件就可以</blockquote></div><br />
到底是哪个目录呢

应该是你的网站目录内的, 你看看哪个, 也很有可能是缓存文件夹
