# 电信光猫 ZXHN F650 超级密码


产品型号ZXHN F650(GPON ONU)<br />
软件版本号V2.0.3P1T2<br />
<br />
请问这个版本的超级密码能搞么？刚装了条电信宽带，要趁热打铁。<br />
（网上找了一些方法，U盘那种的尝试过了，不行）

拆机飞线编程器<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
<br />
电信猫的超级密码不都是统一的嘛，像我们大深圳电信就从来不会去改

需要你自己本地区抓包破解的！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

哪这么多事 打电话给装宽带的师傅问他超级密码多少

给10000打电话他们告诉你<img id="aimg_P5tnp" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 tsubasa 于 2020-10-23 17:33 编辑 </i><br />
<br />
测试telnet是否开放，如果在线未开放，尝试拔光纤，关电源等30秒再开，如果能进telnet了，你懂的了<br />
没拿到密码前，不要插入光纤，否则马上断链<br />
<br />
如果上面的都不行：改光猫区域版本到默认版本，等光猫重启完了，再次改回你所在的区域，尝试上面的步骤<br />
<br />
<br />
前提是你已经注册好光猫，绑定好LOID，记录好你所有的信息，因为不要再用重注册下发的方式来玩了，下发后，又会变了<br />
<br />
<br />
其实中兴的猫算是最简单的了……<img id="aimg_Ua1x9" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

万能的某宝

我也是f650，看用户端登陆界面/cgi-bin/luci/竟然是openwrt的魔改版，不过师傅来装的时候已经让他改好桥接了<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9342128&amp;ptid=757681" target="_blank"><font color="#999999">MoeWang 发表于 2020-10-23 17:39</font></a></font><br />
我也是f650，看用户端登陆界面/cgi-bin/luci/竟然是openwrt的魔改版，不过师傅来装的时候已经让他改好桥接 ...</blockquote></div><br />
改桥接有什么好处？<img id="aimg_eH0JC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9342178&amp;ptid=757681" target="_blank"><font color="#999999">shares 发表于 2020-10-23 17:48</font></a></font><br />
改桥接有什么好处？</blockquote></div><br />
可以用路由器拨号，性能更强...<img id="aimg_bISag" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
