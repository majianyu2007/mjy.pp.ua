# 使用frp内网穿透，个人宽带不使用80,443等端口建站可以么


<font size="6">腾讯云还有半年到期，自己手上有小主机，想配合www.natfrp.com做家庭建站，手上有北岸过的域名和一个没有北岸的域名，网站上都是一些正常的资源，风险大吗？</font>

可以，但是个人ip对外提供服务就是WF

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341274&amp;ptid=757616" target="_blank"><font color="#999999">pengxp1996 发表于 2020-10-23 15:03</font></a></font><br />
可以，但是个人ip对外提供服务就是WF</blockquote></div><br />
建站感觉对外都是提供服务<img src="static/image/smiley/default/titter.gif" smilieid="9" border="0" alt="" />

frp使用的不是服务器IP中转的嘛，中转服务器IP不是国内的不需要北岸啊<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

可以的。。以前我也这么干过

感觉没有被盯上就没啥事，不要放啥作死的内容

我的签名就是这么干的

国内服务器你还是需要北岸,北岸服务器那边就好了<br />
<br />
<br />
frp最好想办法加密下连接,貌似有选项的<img id="aimg_xV1oR" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

可以吧 这样运营商也发现不了 我感觉最好的方法就是找个高位端口 然后弄个小鸡反向代理 再弄个只允许小鸡ip访问

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9341413&amp;ptid=757616" target="_blank"><font color="#999999">dragonfsky 发表于 2020-10-23 15:26</font></a></font><br />
可以吧 这样运营商也发现不了 我感觉最好的方法就是找个高位端口 然后弄个小鸡反向代理 再弄个只允许小鸡ip ...</blockquote></div><br />
弄个只允许小鸡ip，你这个建议非常好
