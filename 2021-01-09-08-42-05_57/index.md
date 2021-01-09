# 腾讯云服务器安装BBR Plus 过程中失联


<i class="pstatus"> 本帖最后由 kra 于 2020-10-30 18:15 编辑 </i><br />
<br />
脚本是会动内核的，有卸载全部内核的过程。脚本安装完成后，应该检查内核是否还在。。。。<br />
<br />
可以参考不卸载内核的版本，一般不会有问题，百试百灵，不会失联。<br />
<br />
如下的：<br />
不卸载内核<br />
wget -N --no-check-certificate &quot;https://github.000060000.xyz/tcpx.sh&quot; &amp;&amp; chmod +x tcpx.sh &amp;&amp; ./tcpx.sh<br />
或<br />
wget -N &quot;https://github.000060000.xyz/tcpx.sh&quot; &amp;&amp; chmod +x tcpx.sh &amp;&amp; ./tcpx.sh

换centos8也不会太占内存
