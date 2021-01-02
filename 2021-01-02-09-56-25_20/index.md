# 第一次遇到这种错误，取消SSL就好了


<img id="aimg_XPSwG" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://www.png8.com/imgs/2020/11/7b9492492784c8c8.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
<br />
<br />
看看大佬们怎么说。。。。

用的老协议吧。

SSL3, TLSv1, TLSv1.1 将不再受支持<br />
<br />
弱密钥交换机制亦将不受支持

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9452547&amp;ptid=766566" target="_blank"><font color="#999999">菜单 发表于 2020-11-14 12:15</font></a></font><br />
用的老协议吧。</blockquote></div><br />
腾讯哪儿生成的啊

我也遇到过是套CF之后，跟CF有关，没套那就是你ssl设置有问题，80%是你设置有问题，给你发个原版吧，直接复制替换解决<br />
<br />
<br />
&nbsp; &nbsp; ssl_protocols&nbsp; &nbsp;TLSv1.2 TLSv1.3;<br />
&nbsp; &nbsp; ssl_ciphers ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES128-GCM-SHA256<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES256-GCM-SHA384:ECDHE-ECDSA-AES128-SHA256:ECDHE-RSA-AES128-SHA256:ECDHE-ECDSA-AES128-SHA:ECDHE-RSA-AES256-SHA384:ECDHE-RSA-AES128-SHA:ECDHE-ECDSA-AES256-SHA384:ECDHE-ECDSA-AES256-SHA:ECDHE-RSA-AES256-SHA<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES128-SHA256<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES128-SHA<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES256-SHA256<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />HE-RSA-AES256-SHA:ECDHE-ECDSA-DES-CBC3-SHA:ECDHE-RSA-DES-CBC3-SHA:EDH-RSA-DES-CBC3-SHA:AES128-GCM-SHA256:AES256-GCM-SHA384:AES128-SHA256:AES256-SHA256:AES128-SHA:AES256-SHA<img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />ES-CBC3-SHA:!DSS;
