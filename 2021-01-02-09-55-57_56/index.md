# HZ的4TX2机器，安装问题


recuse选择RAID0<br />
但是/只分配2T /HOME分配6T<br />
如何设置才能/分配8T呢

删除分区，然后扩大分区<img id="aimg_AfzK2" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

root@Ubuntu-1804-bionic-64-nextcloud ~ # df -H<br />
Filesystem&nbsp; &nbsp;&nbsp; &nbsp;Size&nbsp;&nbsp;Used Avail Use% Mounted on<br />
udev&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 34G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp; &nbsp;34G&nbsp; &nbsp;0% /dev<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;6.8G&nbsp;&nbsp;783k&nbsp;&nbsp;6.8G&nbsp; &nbsp;1% /run<br />
/dev/md2&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;2.2T&nbsp;&nbsp;2.8G&nbsp;&nbsp;2.1T&nbsp; &nbsp;1% /<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;34G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp; &nbsp;34G&nbsp; &nbsp;0% /dev/shm<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;5.3M&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;5.3M&nbsp; &nbsp;0% /run/lock<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;34G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp; &nbsp;34G&nbsp; &nbsp;0% /sys/fs/cgroup<br />
/dev/md3&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;5.8T&nbsp; &nbsp;93M&nbsp;&nbsp;5.5T&nbsp; &nbsp;1% /home<br />
/dev/md1&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;511M&nbsp; &nbsp;79M&nbsp;&nbsp;406M&nbsp;&nbsp;17% /boot<br />
tmpfs&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;6.8G&nbsp; &nbsp;&nbsp;&nbsp;0&nbsp;&nbsp;6.8G&nbsp; &nbsp;0% /run/user/0<br />
请问如何删除扩大啊

重新安装系统，可以设置分区啊，当然也可以直接修改，看下别人写的https://note.guotianyu.cn/linux/centos7-move-home-to-root.html

安装时选择LVM

安装的时候把其他3个硬盘都注释掉, 只安装到第一个上面.<br />
装好后再手动挂载.<br />
<br />


lvm扩容

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9402676&amp;ptid=762413" target="_blank"><font color="#999999">轻风伴梦 发表于 2020-11-4 17:28</font></a></font><br />
重新安装系统，可以设置分区啊，当然也可以直接修改，看下别人写的https://note.guotianyu.cn/linux/centos ...</blockquote></div><br />
我是乌班图<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # xfs_growfs /dev/centos/root&nbsp;&nbsp;<br />
xfs_growfs: /dev/centos/root is not a mounted XFS filesystem<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # df -h lvremove /dev/home ^C<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # lvremove /dev/home <br />
&nbsp;&nbsp;Volume group &quot;home&quot; not found<br />
&nbsp;&nbsp;Cannot process volume group home<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # lvremove /dev/UBUNTU/HOME<br />
&nbsp;&nbsp;Volume group &quot;UBUNTU&quot; not found<br />
&nbsp;&nbsp;Cannot process volume group UBUNTU<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # lvremove /dev/ubuntu/home<br />
&nbsp;&nbsp;Volume group &quot;ubuntu&quot; not found<br />
&nbsp;&nbsp;Cannot process volume group ubuntu<br />
root@Ubuntu-1804-bionic-64-nextcloud ~ # <br />
<br />
好像不好使。

把home分区那行代码删掉

然后把/分区分配空间改为all
