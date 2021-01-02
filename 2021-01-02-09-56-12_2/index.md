# 怎么从本里SSL证书文件里检测到有效期？


请教大佬们

eheh.org添加证书后可以马上看到明细，还可以预警通知

帮顶，这个问题好高端<br />
<br />
技术大佬们回答吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

自己生成的还不知道有效期多久？<br />
win系统直接双击证书<br />
其他系统要么直接cpoy证书代码线上验证<br />
要么配置一下用curl、openssl等都可以验证有效期

openssl或者windows双击<br />
<br />
或者找X509在线解析工具

对 SSL 公钥证书解 base64，可以得到生效时间和过期时间的 Unix 时间<img id="aimg_AYYv7" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

好了<br />
openssl x509 -in <a href="http://www.xxx.com.pem" target="_blank">www.xxx.com.pem</a> -noout -dates

<div class="quote"><blockquote><font color="#999999">h20 发表于 2020-11-3 18:17</font><br />
<font color="#999999">openssl或者windows双击<br />
<br />
或者找X509在线解析工具</font></blockquote></div><br />
win双击？&nbsp;&nbsp;我回去试看看&nbsp;&nbsp;是crt 还是key

<i class="pstatus"> 本帖最后由 iks 于 2020-11-4 10:21 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9399847&amp;ptid=761932" target="_blank"><font color="#999999">1594959462 发表于 2020-11-4 10:06</font></a></font><br />
win双击？&nbsp;&nbsp;我回去试看看&nbsp;&nbsp;是crt 还是key</blockquote></div><br />
<br />
只有证书公钥会带有效期<br />
<br />
数字证书就是对密钥对公钥签字并补充信息(签名者使用者使用期间和其它扩展)

<div class="quote"><blockquote><font color="#999999">iks 发表于 2020-11-4 10:19</font><br />
<font color="#999999">只有证书公钥会带有效期<br />
<br />
数字证书就是对密钥对公钥签字并补充信息(签名者使用者使用期间和其它扩展) ...</font></blockquote></div><br />
惨了&nbsp;&nbsp;知识范畴以外。。。下来了解了解
