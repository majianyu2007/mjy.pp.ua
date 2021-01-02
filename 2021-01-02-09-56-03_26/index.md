# 请教大家一个旁路由设置的问题


<i class="pstatus"> 本帖最后由 fule 于 2020-11-4 23:47 编辑 </i><br />
<br />
大环境:<br />
学校校园网,有深蓝认证.目前宿舍只有一个宽带插口,就是可以插网线的一个口<br />
目前配置如下:<br />
1.N1盒子已经刷好openwrt,设置地址为192.168.0.102<br />
2.N1盒子通过网线连接路由器的LAN口,路由器WAN口接到了宿舍宽带插口,现在我的电脑连接路由器可以上网.<br />
<br />
3.下面是我路由器的截图<br />
<img id="aimg_tOvsn" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://kyun.ltyuanfang.cn/tc/2020/11/04/ffb381a40e20e.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_eqb4z" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://kyun.ltyuanfang.cn/tc/2020/11/04/97f89f85ef6e4.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
4.下面是我n1的截图<br />
<img id="aimg_Lvp7O" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://kyun.ltyuanfang.cn/tc/2020/11/04/1e5da1400017b.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
现在遇到的问题是:<br />
现在我的电脑连接路由器可以上网.,但是访问openwrt的192.168.0.102访问不了,ping这个地址显示无法访问目标主机.<br />
此外,我链接openwrt的这个wifi,也进不去192.168.0.102,也就是openwrt的后台

<a href="https://www.hostloc.com/home.php?mod=space&amp;uid=41824" target="_blank">@popo2731</a> 刚回了啥没看到

大水b现在还在上学，不是退休了吗<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

这问进不去n1后台贴一个拨号路由器的图，真当我们神仙？

暴露学校了。。。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404207&amp;ptid=762552" target="_blank"><font color="#999999">花样撸管冠军 发表于 2020-11-4 23:19</font></a></font><br />
这问进不去n1后台贴一个拨号路由器的图，真当我们神仙？</blockquote></div><br />
<img src="static/image/smiley/yct/016.gif" smilieid="51" border="0" alt="" />我也不懂啊呜呜呜,n1后台啥也没改动,九八地址改成了192.168.0.102

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404214&amp;ptid=762552" target="_blank"><font color="#999999">fatal 发表于 2020-11-4 23:20</font></a></font><br />
暴露学校了。。。</blockquote></div><br />
没事,学校跨市三个地块,网都显示一个地

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9404218&amp;ptid=762552" target="_blank"><font color="#999999">fule 发表于 2020-11-4 23:20</font></a></font><br />
我也不懂啊呜呜呜,n1后台啥也没改动,九八地址改成了192.168.0.102</blockquote></div><br />
简单看了一下问题，应该是主路由跟N1不同网段

N1直插电脑进去看看

你这都不是一个IP段啊，要把N1的地址设置成与路由分配IP一个子网的，而且不要冲突<img id="aimg_m3qym" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
