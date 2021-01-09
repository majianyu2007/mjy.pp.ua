# 进不了系统了，咋破啊


grub是一个系统引导器，是Linux常用的软件；一般win不用这个东西引导用的是ntldr如果我没记错的话；<br />
出现了这个玩意说明你硬盘启动时最先找到的是grub，但是grub一般会根据事先写好的配置文件来继续引导你的系统，如果配置有问题（比如找不到引导文件分区之类的）就会进入你截图的这个shell<br />
<br />
如果你现在硬盘上有Linux系统并且还能进去的话，可以用命令重建引导(#2的大佬给出了)；<br />
没有的话，应该是之前装Linux留下的或者什么玩意给你搞上去的grub。确定windows没删的话应该可以改grub配置文件使之默认引导windows，然而有些麻烦<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /> 因为不知道你配置文件在哪也不知道你哪个分区上是windows(我是单给grub一个区的，但似乎它也可以放在引导扇区里这就不好改了)<br />
<br />
最后，要不还是进PE找个软件修复win引导吧。。。

引导的问题

多大点事，塞一张win10安装光盘进去，选择光盘启动，以后全部都下一步就好了

多大点事情，进pe 用直接这个&nbsp;&nbsp;重置下引导就行了<br />
<img id="aimg_kOqQh" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://www.diskgenius.cn/public/images/logo-diskgenius.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

PE重装 另 远离国内全家桶

换一台新的电脑，完美！

pe下重装即可<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

grub都不知道哪来的话 建议直接重装吧

以前也遇到过，在PE里面修复一下引导就行了

楼上正解，修复后进系统发现成盗版了
