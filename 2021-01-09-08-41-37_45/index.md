# centos7装虚拟机的话简单不？


求个大佬给个初级教程，没弄过，只弄过win的hyper

centos 装 win虚拟机么。。。。<img id="aimg_OAO3M" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

简单，iso直接跑

yum install -y qemu-kvm libvirt virt-install bridge-utils<br />
 lsmod |grep kvm<br />
启动libvirtd守护进程<br />
systemctl start libvirtd<br />
systemctl status libvirtd<br />
安装虚拟机<br />
首先需要下载一个镜像文件到母机本地<br />
我们的KVM虚拟机将要安装CentOS系统，于是到CentOS官网找一个镜像的下载链接，使用wget命令下载到本地<br />
之前测试将镜像下载到/root目录，结果安装开始时提示无法读取镜像文件，为了避免权限问题，我们将镜像文件下载到/home目录<br />
wget http://mirrors.163.com/centos/7.5.1804/isos/x86_64/CentOS-7-x86_64-Minimal-1804.iso -P /home/<br />
<br />
执行安装虚拟机命令：<br />
virt-install \<br />
--virt-type=kvm \<br />
--name=kvm-1 \<br />
--vcpus=2 \<br />
--memory=2048 \<br />
--location=/home/CentOS-7-x86_64-Minimal-1804.iso \<br />
--disk path=/data/vms/kvm-1.qcow2,size=15,format=qcow2 \<br />
--network bridge=virbr0 \<br />
--graphics none \<br />
--extra-args='console=ttyS0' \<br />
--force<br />
参数解析：<br />
--name=kvm-1 　　虚拟机名字为kvm-1<br />
--vcpus=2 　　 　&nbsp; &nbsp;2个虚拟CPU核心<br />
--memory=2048&nbsp; &nbsp;&nbsp; &nbsp;2G内存<br />
--disk path=/data/vms/kvm-1.qcow2,size=15,format=qcow2 　　虚拟机硬盘文件所在目录及名字，大小为15G，格式为qcow2，此参数会自动生成该硬盘文件在对应目录<br />
--network bridge=virbr0 　　 虚拟机桥接用的网卡，不一定是这个名字，在母机上用ifconfig查看实际名字 （这里默认使用的是NAT模式，如果要使用Bridge模式，请参考另外一篇文章）<br />
如果一切正常，会进入安装iso安装界面。<br />
上面的设置跟在图形界面安装操作一样，分别进去设置一下就可以继续安装了，设置完如下<br />
然后敲b开始进行安装，成功安装到最后页面：<br />
回车后虚拟机会从开机界面一直进入到登陆界面，输入root和密码就登陆进了虚拟机系统<br />
<br />
退出虚拟机回到母机系统<br />
同时按Ctrl+]<br />
重新连接虚拟机<br />
virsh console kvm-1<br />
KVM 操作虚拟机常用命令：<br />
列出所有的虚拟机<br />
virsh list --all<br />
显示虚拟机信息<br />
virsh dominfo kvm-1<br />
显示虚拟机内存和cpu的使用情况<br />
yum install virt-top -y<br />
virt-top<br />
显示虚拟机分区信息<br />
virt-df kvm-1<br />
关闭虚拟机（shutodwn）<br />
virsh shutdown kvm-1<br />
启动虚拟机<br />
virsh start kvm-1<br />
设置虚拟机（kvm-1）跟随系统自启<br />
virsh autostart kvm-1<br />
关闭虚拟机自启<br />
virsh autostart --disable kvm-1<br />
删除虚拟机<br />
virsh undefine kvm-1

https://www.icabbs.com/thread-354-1-1.html

谢谢，等下我试试

试试Nano,安装后图形界面操作:https://www.xiaoz.me/archives/14842
