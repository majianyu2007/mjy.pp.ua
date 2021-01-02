# 百思不得其解，Navicat连接mysql添加了权限了为何保存不了


如图<br />
<br />
我创建用户后给用户授权，可以登录删除数据库<br />
<br />
但是我想用 这个用户再去创建一个&nbsp;&nbsp;新用户1<br />
<br />
然后保存新用户 1的权限 就提示这样<br />
<br />
<br />
grant all privileges on *.* to `username`@`%` identified by 'pwd';<br />
UPDATE mysql.user SET Grant_priv='Y' WHERE User = 'username';<br />
<br />
<img id="aimg_mFEk8" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/25/wFK94q2NiAWIOpt.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

刷新 配置 

<i class="pstatus"> 本帖最后由 朕的大清完了？ 于 2020-11-25 14:15 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9514960&amp;ptid=771209" target="_blank"><font color="#999999">不眠飞行 发表于 2020-11-25 13:58</font></a></font><br />
刷新 配置</blockquote></div><br />
<br />
刷新过权限&nbsp;&nbsp;flush privileges;<br />
还是那样<br />
<br />
解决了，重启下sql 就好了 <img src="static/image/smiley/yct/002.gif" smilieid="30" border="0" alt="" /> <br />
<br />
重启解决一切<img src="static/image/smiley/yct/005.gif" smilieid="35" border="0" alt="" /> 
