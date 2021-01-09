# 使用frp内网穿透，个人宽带不使用80,443等端口建站可以么


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341776&amp;ptid=757616" target="_blank"><font color="#999999">lxyer 发表于 2020-10-23 16:29</font></a></font><br />
弄个只允许小鸡ip，你这个建议非常好</blockquote></div><br />
这个是论坛大佬教的 他说他弄了个论坛就是这么搞的 还挺好 我准备以后也试试

打算弄一下

就算做正常内容，也是怕哪天就被抓去写保证书了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9349938&amp;ptid=757616" target="_blank"><font color="#999999">爱吃醋的醋醋 发表于 2020-10-25 14:59</font></a></font><br />
就算做正常内容，也是怕哪天就被抓去写保证书了</blockquote></div><br />
看natfrpQQ群里非常多的人这样建站

那干嘛不直接建在小鸡上

你都中转了谁管你啊

frp和个人宽带之间走的根本不是web协议，甚至可以走kcp协议，所以完全不用担心

你都中转了谁管你啊

建站对外访问肯定是违法的 

没有任何问题，你限制得只允许服务器访问，肯定是可以的。<br />
但是如果你过了SDN之类的设备，等于是无用……会有协议流量判定<img id="aimg_Q6bU1" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
