# 关于SSL证书的奇怪问题


<i class="pstatus"> 本帖最后由 19930618 于 2020-10-29 10:20 编辑 </i><br />
<br />
我今天vx公众号上访问：https://wxjj.scienmedia.com/。提示证书存在问题<br />
然后我用ios自带的safari和chrome上也是提示证书异常<br />
可我在PC端的chrome上访问提示证书有效。<br />
用myssl.com检测，提示证书被吊销<br />
我就不信邪，把chrome更新到最新。。还是证书有效。。<br />
后来我用IE。。发现连IE都报证书已被吊销。。<br />
可我的PC端的chrome始终提示是有效的。。奇怪<br />
<br />
<br />
<br />
-----<br />
10：19更新：发现chrome也提示证书无效了。。。chrome证书有效性检测反应慢半拍啊

<i class="pstatus"> 本帖最后由 h20 于 2020-10-29 10:31 编辑 </i><br />
<br />
垃圾chrome是不查ocsp的<br />
<br /><div class="blockcode"><div id="code_pPX"><ol><li><br /><li>OCSP Request Data:<br /><li>&nbsp; &nbsp; Version: 1 (0x0)<br /><li>&nbsp; &nbsp; Requestor List:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Certificate ID:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Hash Algorithm: sha1<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Issuer Name Hash: 978B4716E5B0F658BAE69DAB1689B8363AE3C3A6<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Issuer Key Hash: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; Serial Number: 074FDC8F3FB80B978E39A4AA24F411DC<br /><li>&nbsp; &nbsp; Request Extensions:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;OCSP Nonce:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;0410DFBDF5A7DBEAD3829A8B53FB259E31B2<br /><li>OCSP Response Data:<br /><li>&nbsp; &nbsp; OCSP Response Status: successful (0x0)<br /><li>&nbsp; &nbsp; Response Type: Basic OCSP Response<br /><li>&nbsp; &nbsp; Version: 1 (0x0)<br /><li>&nbsp; &nbsp; Responder Id: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp; Produced At: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp; Responses:<br /><li>&nbsp; &nbsp; Certificate ID:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Hash Algorithm: sha1<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Issuer Name Hash: 978B4716E5B0F658BAE69DAB1689B8363AE3C3A6<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Issuer Key Hash: 55744FB2724FF560BA50D1D7E6515C9A01871AD7<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;Serial Number: 074FDC8F3FB80B978E39A4AA24F411DC<br /><li>&nbsp; &nbsp; Cert Status: revoked<br /><li>&nbsp; &nbsp; Revocation Time: Oct 21 01:44:04 2020 GMT<br /><li>&nbsp; &nbsp; This Update: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp; Next Update: Nov&nbsp;&nbsp;4 14:59:59 2020 GMT<br /><li><br /><li>&nbsp; &nbsp; Signature Algorithm: sha256WithRSAEncryption<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;70:e5:0a:f4:96:45:14:ee:bf:2f:4e:51:24:3a:a6:d8:db:17:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;e3:96:e6:31:36:09:09:99:a7:16:fa:f5:46:ce:d9:f8:ea:c9:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;70:df:f8:0e:ca:44:3f:03:be:2a:0f:59:a5:f1:dc:6e:af:b5:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;69:bc:c7:cb:9e:0e:a7:24:02:a3:fe:20:17:2e:ec:80:85:fd:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;a8:68:c7:68:33:02:12:51:d9:d5:c9:99:78:bc:60:7a:c7:f6:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;41:c7:80:d2:3f:f1:4a:65:96:5b:40:64:eb:75:cf:15:91:64:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;3e:78:4a:11:f6:9d:ef:68:c8:95:26:b7:8e:76:d8:62:36:15:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;ce:f0:a3:22:91:5c:bd:91:a4:7b:7b:7e:bf:fa:5a:f3:78:40:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;2c:81:a8:a4:17:c6:8f:11:dd:6b:3f:4a:4a:2f:85:84:7b:29:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;b5:9d:f7:38:55:34:e3:f2:33:23:fc:14:c9:f9:07:5a:27:fc:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;c1:ab:f5:5d:9f:8a:a2:02:16:cd:5c:af:cd:f0:b6:27:97:a7:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;4c:cc:cd:9d:95:54:db:aa:ae:05:c4:ae:a4:28:65:6a:31:ac:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;32:49:d2:6a:56:a3:a7:10:b3:d2:84:fe:ac:9e:7a:8a:26:d7:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;21:3e:02:09:a5:30:e8:0e:4f:90:a2:3d:3e:6f:7f:1d:f8:6c:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;b5:e2:2b:d2<br /><li>WARNING: no nonce in response<br /><li>Response verify OK<br /><li>1.cer: revoked<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;This Update: Oct 28 15:44:59 2020 GMT<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Next Update: Nov&nbsp;&nbsp;4 14:59:59 2020 GMT<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;Revocation Time: Oct 21 01:44:04 2020 GMT<br /><li></ol></div><em onclick="copycode($('code_pPX'));">复制代码</em></div><br />
<br />
Cert Status: revoked<br />
Revocation Time: Oct 21 01:44:04 2020 GMT

这么奇怪，那推荐换个证书

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367828&amp;ptid=759693" target="_blank"><font color="#999999">tir 发表于 2020-10-29 09:59</font></a></font><br />
这么奇怪，那推荐换个证书</blockquote></div><br />
主要不是我的网站。。是无锡交警。。我想上去查查违章

因为chrome不会去检查证书是否被吊销，只要还在有效期内，并且是信任的ca发布就默认承认有效，你遇到的就是这样

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367872&amp;ptid=759693" target="_blank"><font color="#999999">By小酷 发表于 2020-10-29 10:09</font></a></font><br />
因为chrome不会去检查证书是否被吊销，只要还在有效期内，并且是信任的ca发布就默认承认有效，你遇到的就是 ...</blockquote></div><br />
那这样是不是不安全啊。假设我的私钥泄露了，我把这个证书吊销了。可chrome还是提示证书有效。。很大的安全隐患啊

<div class="quote"><blockquote><font color="#999999">19930618 发表于 2020-10-29 10:12</font><br />
<font color="#999999">那这样是不是不安全啊。假设我的私钥泄露了，我把这个证书吊销了。可chrome还是提示证书有效。。很大的安 ...</font></blockquote></div><br />
chrome默认设置就是不去检查，说是为了速度，这个没办法，证书私钥丢失也要匹配域名，问题不大

<i class="pstatus"> 本帖最后由 蓝瘦香菇 于 2020-10-29 10:19 编辑 </i><br />
<br />
用的哪的证书，应该是服务器端没设置好<img src="static/image/smiley/yct/007.gif" smilieid="46" border="0" alt="" /> <br />
是不是缺少了ca证书

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367898&amp;ptid=759693" target="_blank"><font color="#999999">By小酷 发表于 2020-10-29 10:14</font></a></font><br />
chrome默认设置就是不去检查，说是为了速度，这个没办法，证书私钥丢失也要匹配域名，问题不大 ...</blockquote></div><br />
私钥丢失+DNS污染<br />
或者中间人攻击问题就大了

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367918&amp;ptid=759693" target="_blank"><font color="#999999">19930618 发表于 2020-10-29 10:16</font></a></font><br />
私钥丢失+DNS污染<br />
或者中间人攻击问题就大了</blockquote></div><br />
<br />
中间人攻击不会用合法证书(由CA签发)

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9367928&amp;ptid=759693" target="_blank"><font color="#999999">iks 发表于 2020-10-29 10:18</font></a></font><br />
中间人攻击不会用合法证书(由CA签发)</blockquote></div><br />
刚chrome也提示证书无效了。。。
