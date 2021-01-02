# 黑五变态机有救，可以用NFS挂载一个僚机


<i class="pstatus"> 本帖最后由 sRGB 于 2020-10-22 23:04 编辑 </i><br />
<br />
<img id="aimg_FE2Kc" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/22/VltEuXR1oYhdIxN.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
水牛城 3G 硬盘的 机器 ，挂载亚特兰大 32G盘的机器，网盘速度 有 9-10M/s<br />
<br /><div class="blockcode"><div id="code_fnk"><ol><li># NFS 服务端安装设置<br /><li>apt install nfs-kernel-server -y<br /><li><br /><li>mkdir nfsdir<br /><li><br /><li>echo '/root/nfsdir&nbsp;&nbsp;10.0.8.0/24(rw,sync,no_root_squash)'&nbsp;&nbsp;&gt;&gt; /etc/exports<br /><li><br /><li>sudo /etc/init.d/nfs-kernel-server restart<br /><li><br /><li># 或者<br /><li>systemctl&nbsp;&nbsp;restart&nbsp;&nbsp;nfs-kernel-server<br /><li><br /><li>showmount -e<br /><li>Export list for kvm-VirMach:<br /><li>/root/nfsdir 10.0.8.0/24<br /><li><br /><li># NFS 客户端安装使用<br /><li>apt install nfs-common -y<br /><li><br /><li>mkdir /mnt/nfsdir -p<br /><li>mount -t nfs 10.0.8.1:/root/nfsdir /mnt/nfsdir<br /><li>df -h<br /><li>cd /mnt/nfsdir<br /><li><br /><li>dd if=/dev/zero of=1.bin bs=1M count=100<br /><li><br /><li>dd if=/dev/zero of=1.bin bs=1M count=1024<br /><li><br /><li></ol></div><em onclick="copycode($('code_fnk'));">复制代码</em></div><br />
以上配置 Debian 10 配置通过测试，虚拟网络 使用WG搭建，服务端和客户端都用这个脚本搭建<br />
客户端 自行修改配置文件<br />
<br /><div class="blockcode"><div id="code_mpE"><ol><li># One-Step Automated Install WireGuard Script<br /><li>wget -qO- https://git.io/wireguard.sh | bash</ol></div><em onclick="copycode($('code_mpE'));">复制代码</em></div><br />
<br />
NFS就是Network File System的缩写，它最大的功能就是可以通过网络，让不同的机器、不同的操作系统可以共享彼此的文件。<br />
<br />
​ NFS服务器可以让PC将网络中的NFS服务器共享的目录挂载到本地端的文件系统中，而在本地端的系统中来看，那个远程主机的目录就好像是自己的一个磁盘分区一样，在使用上相当便利；<br />
<br />
https://blog.csdn.net/qq_38265137/article/details/83146421

会玩，这算是压榨到极致了！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

看起来不错啊！

那如果水牛城挂载水牛城的呢？速度会不会更快一点。

榨干

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9338528&amp;ptid=757390" target="_blank"><font color="#999999">yanaxiao 发表于 2020-10-22 22:47</font></a></font><br />
那如果水牛城挂载水牛城的呢？速度会不会更快一点。</blockquote></div><br />
AWS 机器测试 能有 50-60M<br />
自己硬盘 75M

如果内联通那就好了

真会玩

挂个2欧试试
