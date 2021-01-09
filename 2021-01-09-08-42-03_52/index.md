# 关于SSL证书的奇怪问题


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367946&amp;ptid=759693" target="_blank"><font color="#999999">19930618 发表于 2020-10-29 10:21</font></a></font><br />
刚chrome也提示证书无效了。。。</blockquote></div><br />
这个域名不像正规域名，目测被 CRL 和 OCSP 吊销<br />
<br />
另，Chrome 去拉 CRL 的频率比较低，你得等 CRL 过期或清除 Chrome 缓存来让 Chrome 去拉取 CRL

<i class="pstatus"> 本帖最后由 h20 于 2020-10-29 10:31 编辑 </i><br />
<br />
垃圾chrome是不查ocsp的<br />
<br /><div class="blockcode"><div id="code_ek0"><ol><li><br /><li>OCSP Request Data:<br /><li>&nbsp; &nbsp; Version: 1 (0x0)<br /><li>&nbsp; &nbsp; Requestor List:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Certificate ID:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Hash Algorithm: sha1<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Issuer Name Hash: 978B4716E5B0F658BAE69DAB1689B8363AE3C3A6<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Issuer Key Hash: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Serial Number: 074FDC8F3FB80B978E39A4AA24F411DC<br /><li>&nbsp; &nbsp; Request Extensions:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;OCSP Nonce:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;0410DFBDF5A7DBEAD3829A8B53FB259E31B2<br /><li>OCSP Response Data:<br /><li>&nbsp; &nbsp; OCSP Response Status: successful (0x0)<br /><li>&nbsp; &nbsp; Response Type: Basic OCSP Response<br /><li>&nbsp; &nbsp; Version: 1 (0x0)<br /><li>&nbsp; &nbsp; Responder Id: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp; Produced At: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp; Responses:<br /><li>&nbsp; &nbsp; Certificate ID:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Hash Algorithm: sha1<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Issuer Name Hash: 978B4716E5B0F658BAE69DAB1689B8363AE3C3A6<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Issuer Key Hash: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Serial Number: 074FDC8F3FB80B978E39A4AA24F411DC<br /><li>&nbsp; &nbsp; Cert Status: revoked<br /><li>&nbsp; &nbsp; Revocation Time: Oct 21 01:44:04 2020 GMT<br /><li>&nbsp; &nbsp; This Update: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp; Next Update: Nov&nbsp;&nbsp;4 14:59:59 2020 GMT<br /><li><br /><li>&nbsp; &nbsp; Signature Algorithm: sha256WithRSAEncryption<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;70:e5:0a:f4:96:45:14:ee:bf:2f:4e:51:24:3a:a6:d8:db:17:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;e3:96:e6:31:36:09:09:99:a7:16:fa:f5:46:ce:d9:f8:ea:c9:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;70:df:f8:0e:ca:44:3f:03:be:2a:0f:59:a5:f1:dc:6e:af:b5:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;69:bc:c7:cb:9e:0e:a7:24:02:a3:fe:20:17:2e:ec:80:85:fd:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;a8:68:c7:68:33:02:12:51:d9:d5:c9:99:78:bc:60:7a:c7:f6:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;41:c7:80:d2:3f:f1:4a:65:96:5b:40:64:eb:75:cf:15:91:64:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;3e:78:4a:11:f6:9d:ef:68:c8:95:26:b7:8e:76:d8:62:36:15:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;ce:f0:a3:22:91:5c:bd:91:a4:7b:7b:7e:bf:fa:5a:f3:78:40:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2c:81:a8:a4:17:c6:8f:11:dd:6b:3f:4a:4a:2f:85:84:7b:29:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;b5:9d:f7:38:55:34:e3:f2:33:23:fc:14:c9:f9:07:5a:27:fc:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;c1:ab:f5:5d:9f:8a:a2:02:16:cd:5c:af:cd:f0:b6:27:97:a7:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;4c:cc:cd:9d:95:54:db:aa:ae:05:c4:ae:a4:28:65:6a:31:ac:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;32:49:d2:6a:56:a3:a7:10:b3:d2:84:fe:ac:9e:7a:8a:26:d7:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;21:3e:02:09:a5:30:e8:0e:4f:90:a2:3d:3e:6f:7f:1d:f8:6c:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;b5:e2:2b:d2<br /><li>WARNING: no nonce in response<br /><li>Response verify OK<br /><li>1.cer: revoked<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;This Update: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Next Update: Nov&nbsp;&nbsp;4 14:59:59 2020 GMT<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Revocation Time: Oct 21 01:44:04 2020 GMT<br /><li></ol></div><em onclick="copycode($('code_ek0'));">复制代码</em></div><br />
<br />
Cert Status: revoked<br />
Revocation Time: Oct 21 01:44:04 2020 GMT

chrome就这样 一般不检查证书是否被吊销 ie什么的访问时候都会检查的

要不。你换个证书吧

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367982&amp;ptid=759693" target="_blank"><font color="#999999">iks 发表于 2020-10-29 10:25</font></a></font><br />
这个域名不像正规域名，目测被 CRL 和 OCSP 吊销<br />
<br />
另，Chrome 去拉 CRL 的频率比较低，你得等 CRL 过期或 ...</blockquote></div><br />
好像是的。我一台电脑的chrome已经提示注销了。还有一台电脑的chrome还是现实证书有效的

 因为chrome不会去检查证书是否被吊销，只要还在有效期内，并且是信任的ca发布就默认承认有效，你遇到的就是这样

ctrl + F5 强制刷新试一下

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9372053&amp;ptid=759693" target="_blank"><font color="#999999">caddy 发表于 2020-10-29 22:17</font></a></font><br />
ctrl + F5 强制刷新试一下</blockquote></div><br />
强制刷新试过，清除缓存也试过

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367928&amp;ptid=759693" target="_blank"><font color="#999999">iks 发表于 2020-10-29 10:18</font></a></font><br />
中间人攻击不会用合法证书(由CA签发)</blockquote></div><br />
<img src="static/image/smiley/yct/014.gif" smilieid="45" border="0" alt="" /> 试着在你签名站上买个SSL 没想到注册会员直接500错误了~

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9373912&amp;ptid=759693" target="_blank"><font color="#999999">气味 发表于 2020-10-30 10:26</font></a></font><br />
试着在你签名站上买个SSL 没想到注册会员直接500错误了~</blockquote></div><br />
没对接支付网关，有需求加微信 KukiSakura <img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" /><img id="aimg_zJ21d" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />
