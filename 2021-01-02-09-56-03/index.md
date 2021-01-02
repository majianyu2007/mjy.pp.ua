# 【90bbs】AWS CloudFront 自选IP实现国内棉被CDN完全手册


<i class="pstatus"> 本帖最后由 Madlifer 于 2020-11-4 12:43 编辑 </i><br />
<br />
防止采集，密码<div class="blockcode"><div id="code_bYS"><ol><li>vicho.vicho</ol></div><em onclick="copycode($('code_bYS'));">复制代码</em></div><br />
<br />
为控制传播速度，今晚6点钟关机下班后255此贴，博客设置密码访问。<br />
<br />
<img id="aimg_Z5WUV" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="229" src="https://i.loli.net/2020/11/04/PKrgxuJ86RUhDSd.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
<img id="aimg_Db9LK" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="328" src="https://i.loli.net/2020/11/04/uv63Na1U54HdeZD.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<br />
AWS提供CloudFront的CDN服务是不支持自选IP的,由于CloudFront边缘节点只提供东南亚导致速度十分捉鸡，甚至不如cloudflare提供的免费服务好用。<br />
<br />
但某大佬意外发现可以通过类似于Cloudflare方式将备用域名Cname到cloudfrontCDN服务器的方式实现自选IP，且AWS在国内部署了不少的边缘节点(未开放)，这就提供了一个可能，即通过自选IP的方式将域名DNS解析到AWS国内边缘节点，实现国内棉被CDN。<br />
<br />
在实现这一操作中，面临以下几个问题：<br />
<br />
1.如何找到AWS在国内的边缘节点<br />
2.如何进行CDN侧的自选IP设置<br />
3.如何实现自动push优选后的IP到DNS上<br />
<br /><div class="quote"><blockquote>本文将全程提供指导以供配置好 1和2、 3需要不少成本所以没做，但是做起来也很简单。<br />
<br />
下一页为链接形式，如果不喜欢，可以不点开</blockquote></div><br />
<br />
<br />
---------<br />
注意，不是完全白女票，CloudFront也是要付费的，只是吃码子情况下付费很低<br />
<br />
而且还是国内节点，所以比较有价值，你懂的。<br />


还以为出了啥新玩法<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" /><br />
点开发现还是老玩意

如果aws starter不能用的话，感觉折腾意义不大

aws早就发现异常了，基本该杀的都杀了。10多块的aws学生账号已经用不了，唯一能用的，就是跟正常账号一样正常计费扣钱了。

谢谢热心分享<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

感谢分享<br />
<br />
<br />
<br />
稍后研究

感谢大佬分享

本来还想搬运走，看来还是不要这么干

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9401014&amp;ptid=762277" target="_blank"><font color="#999999">pengxp1996 发表于 2020-11-4 12:43</font></a></font><br />
本来还想搬运走，看来还是不要这么干</blockquote></div><br />
别搬.棉被还是比较敏感&nbsp;&nbsp;

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9401020&amp;ptid=762277" target="_blank"><font color="#999999">Madlifer 发表于 2020-11-4 12:44</font></a></font><br />
别搬.棉被还是比较敏感</blockquote></div><br />
大家都懂

话说其实WebSocket有没有必要检测？因为好像都不支持Upgrade操作了，以前可以检测的。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9401060&amp;ptid=762277" target="_blank"><font color="#999999">iwktd1220 发表于 2020-11-4 12:51</font></a></font><br />
话说其实WebSocket有没有必要检测？因为好像都不支持Upgrade操作了，以前可以检测的。 ...</blockquote></div><br />
你如果要用来富强肯定要检测，好多节点ws都是废的 5秒断
