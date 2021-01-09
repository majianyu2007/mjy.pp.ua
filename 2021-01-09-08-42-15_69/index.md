# kvm一个不知道是bug还是啥，解决了，给后者少踩坑


桥接虚拟机绑定ip后，设置dns可以上网了，宿主机service network restart后，虚拟机没网，虚拟机内部怎么搞都不行，宿主机virsh shutdown kvm，然后再virsh start kvm 才好使。不知道原理。

宿主机我一般都不动，我没事去service network restart作甚？&nbsp;&nbsp;要是真我去service network restart了出现了这种问题，那么我的解决方案会是重启 ...&nbsp;&nbsp;不过我一般不去动宿主机的！ <img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381513&amp;ptid=760670" target="_blank"><font color="#999999">tir 发表于 2020-10-31 18:31</font></a></font><br />
宿主机我一般都不动，我没事去service network restart作甚？&nbsp;&nbsp;要是真我去service network restart了出现了 ...</blockquote></div><br />
这不是学习嘛，命令自己解决，还没用其他面板。目前基本问题都可以解决了。

？？？？

原因：<br />
1. 重启网络服务的话会关闭网卡，然后再载入网卡配置，如果没有把小鸡的虚拟网卡写入网卡配置里的话，网桥重启是不会加载虚拟机的虚拟网卡的。<br />
2. 一般也不会把小鸡的网卡信息写到宿主机网卡配置里，都是随用随加的，所以重启后小鸡不能上网。<br />
<br />
解决方案：<br />
virsh重启小鸡，kvm启动小鸡的时候会加载配置文件，里面就会有虚拟网卡的信息，会自动加到网卡配置里。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381697&amp;ptid=760670" target="_blank"><font color="#999999">CloudRaft 发表于 2020-10-31 19:26</font></a></font><br />
原因：<br />
1. 重启网络服务的话会关闭网卡，然后再载入网卡配置，如果没有把小鸡的虚拟网卡写入网卡配置里的话 ...</blockquote></div><br />
如果母鸡重启机器的话，是不是也和重启网络一个效果？

我有点好奇cloudraft到底是客服还是专业运维

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9381728&amp;ptid=760670" target="_blank"><font color="#999999">斌斌 发表于 2020-10-31 19:31</font></a></font><br />
如果母鸡重启机器的话，是不是也和重启网络一个效果？</blockquote></div><br />
重启就是关闭机器之后再打开，至于后续开启网络、开机小鸡都是xxx.service来引导执行的。<br />
重启机器肯定会重启网络，但是不仅是重启网络

手写一个ifcfg-br0也没很困难吧
