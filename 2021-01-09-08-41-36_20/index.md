# 企业邮箱收不到微软的邮件怎么回事啊


垃圾箱没有。。。。从腾讯搬迁到阿里云还是这样。。。。<br />
<br />
<br />
<br />
<br />
mail@域名.com&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; 这个我自己在用，也给wordpress网站上绑定了做发信用。。。<br />
<br />
<br />
<br />
<br />
有谁知道的嘛。。。

1、登录阿里邮箱网页版<br />
2、设置<br />
3、账户与安全，检查收信日志<br />
4、邮箱设置，检查反垃圾选项

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9357222&amp;ptid=758780" target="_blank"><font color="#999999">指间的思念 发表于 2020-10-27 08:27</font></a></font><br />
1、登录阿里邮箱网页版<br />
2、设置<br />
3、账户与安全，检查收信日志</blockquote></div><br />
收信日志都没有。。。。没有设置反垃圾。。。

根域名设了CNAME？<img id="aimg_b2dEg" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359772&amp;ptid=758780" target="_blank"><font color="#999999">iks 发表于 2020-10-27 16:06</font></a></font><br />
根域名设了CNAME？</blockquote></div><br />
设置。。。了。。。。但是好像就是个别邮件收不到。我也是客户反馈才发现的。昨天拿来注册微软的浏览器。结果发现我收不到验证码。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359788&amp;ptid=758780" target="_blank"><font color="#999999">312633180 发表于 2020-10-27 16:09</font></a></font><br />
设置。。。了。。。。但是好像就是个别邮件收不到。我也是客户反馈才发现的。昨天拿来注册微软的浏览器。 ...</blockquote></div><br />
不建议根域名CNAME，如果是CNAME到Cloudflare可以一救<img id="aimg_R99l0" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359826&amp;ptid=758780" target="_blank"><font color="#999999">iks 发表于 2020-10-27 16:16</font></a></font><br />
不建议根域名CNAME，如果是CNAME到Cloudflare可以一救</blockquote></div><br />
<br />
我换到阿里云的企业邮箱了。也不行。。日了。。。根域名CNAME是他们要求的。。。&nbsp;&nbsp;<br />
<br />
<br />
拦截日志都没有<br />
<br />
 联系了腾讯的客服。他说可能是没有投递成功。叫我去问下微软。看有没有退信。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9359861&amp;ptid=758780" target="_blank"><font color="#999999">312633180 发表于 2020-10-27 16:27</font></a></font><br />
我换到阿里云的企业邮箱了。也不行。。日了。。。根域名CNAME是他们要求的。。。&nbsp;&nbsp;</blockquote></div><br />
根域名 CNAME 本身就不符合 RFC 规范，理论上收信只要配置 MX 记录就可以了<img id="aimg_SYZGp" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
