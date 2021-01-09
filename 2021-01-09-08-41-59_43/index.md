# 麻烦问下安装完了kvm没办法连接进虚拟机？


麻烦问下安装完了kvm没办法连接进虚拟机？<br />
提示这个<br />
[root@150S276 ~]# virsh console kvm-binbin<br />
Connected to domain kvm-binbin<br />
Escape character is ^]<br />
<br />
刚刚安这个教程做了。重启了。没啥用呢。<br />
<br />
<br />
<br />
解决方法（在虚拟机中做如下操作）<br />
<br />
1、修改&nbsp;&nbsp;/etc/securetty 到最后添加 ttyS0<br />
<br />
&nbsp; &nbsp; echo ttyS0 &gt;&gt; /etc/securetty<br />
<br />
2、修改/etc/inittab 到最后添加&nbsp;&nbsp;S0:12345:respawn:/sbin/agetty/ ttyS0 115200<br />
<br />
&nbsp; &nbsp; echo &quot;S0:12345:respawn:/sbin/agetty/ ttyS0 115200&quot; &gt;&gt; /etc/inittab<br />
<br />
3、修改/etc/grub.conf 或者/etc/grub2.cfg<br />
<br />
在系统配置添加console=ttyS0
