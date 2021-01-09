# 哪位大佬知道SWAP分区怎么释放


不管DD还是面板安装都会分配一个SWAP分区。实际硬盘都不够用了。<br />
<br />
DD脚本是萌咖的。<br />
<br />
注：网上找到的都是释放SWAP文件的。现在问题是SWAP分区。

fdisk吧

<i class="pstatus"> 本帖最后由 Nameless 于 2020-10-30 22:09 编辑 </i><br />
<br />
看到这里想起之前有人私信问我忘记回复了<br />
<br />
google 找 preseed.cfg，看下注释按需改原脚本里的 preseed.cfg 内容。<br />
<br />
或，fdisk 删除所有分区，重建分区，保存退出。<br />
<br />
建议 fdisk 自动化

<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> swapoff -a之后fdisk

swapoff释放swap—fdisk删除swap—resize2fs扩容，再把/etc/fstab里swap那一行删除

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378405&amp;ptid=760390" target="_blank"><font color="#999999">咸鱼咸鱼 发表于 2020-10-30 22:17</font></a></font><br />
swapoff释放swap—fdisk删除swap—resize2fs扩容，再把/etc/fstab里swap那一行删除</blockquote></div><br />
感谢大佬提供建议。最后那句亮了。强迫症必备。

fdisk ，前提条件 swap分区必须在最后一个

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378263&amp;ptid=760390" target="_blank"><font color="#999999">Nameless 发表于 2020-10-30 22:08</font></a></font><br />
看到这里想起之前有人私信问我忘记回复了<br />
<br />
google 找 preseed.cfg，看下注释按需改原脚本里的 preseed.cfg&nbsp;&nbsp;...</blockquote></div><br />
你这个方法昨天试了。然后搞翻车了一个VPS。还得发工单要求重装系统。面板直接无反应了。<br />
<br />
还是删swap分区靠谱。
