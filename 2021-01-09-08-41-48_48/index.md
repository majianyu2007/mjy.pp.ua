# 【记录】Virtualizor 设置内网IP


<div class="blockcode"><div id="code_VPO"><ol><li><br /><li><br /><li>vi /etc/sysconfig/network-scripts/ifcfg-intbr0<br /><li><br /><li>DEVICE=intbr0<br /><li>ONBOOT=yes<br /><li>TYPE=Bridge<br /><li>BOOTPROTO=static<br /><li>IPADDR=192.168.1.1<br /><li>NETMASK=255.255.255.0<br /><li><br /><li><br /><li><br /><li><br /><li><br /><li><br /><li>ifup intbr0<br /><li><br /><li><br /><li><br /><li>显示创建的网桥<br /><li>brctl show<br /><li><br /><li><br /><li><br /><li><br /><li><br /><li>然后在创建vps高级设置和plan里面有设置内网IP个数<br /><li></ol></div><em onclick="copycode($('code_VPO'));">复制代码</em></div><br />
<br />
<br />
<img id="aimg_mnVPI" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://www.zaixiakefu.com/storage/files/c1Is07wYSzUziwmSOX0IoWdZIeYHeQgSei5Mc3U0.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

顶
