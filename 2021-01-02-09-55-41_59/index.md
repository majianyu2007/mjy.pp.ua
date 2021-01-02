# 有什么 curl查询指定IP 的接口吗？


<i class="pstatus"> 本帖最后由 O₂ 于 2020-10-25 16:31 编辑 </i><br />
<br />
curl myip.ipip.net<br />
当前 IP：x.x.x.x&nbsp;&nbsp;来自于：中国 XX XX&nbsp;&nbsp;联通<br />
<br />
myip.ipip.net<br />
和<br />
ip.sb<br />
<br />
都只能查本地的IP<br />
我想找一个能查指定IP的<img src="static/image/smiley/yct/005.gif" smilieid="35" border="0" alt="" /> 

很明显，不可能的，付费吧

curl是服务器ip

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350232&amp;ptid=758302" target="_blank"><font color="#999999">h20 发表于 2020-10-25 16:10</font></a></font><br />
很明显，不可能的，付费吧</blockquote></div><br />
<br />
找到一个<br />
<br />
curl www.cip.cc/1.1.1.1&nbsp; &nbsp;&nbsp; &nbsp;<br />
 <br />
IP&nbsp; &nbsp; &nbsp; &nbsp; : 1.1.1.1<br />
地址&nbsp; &nbsp; &nbsp; &nbsp; : CLOUDFLARE.COM&nbsp;&nbsp;CLOUDFLARE.COM<br />
<br />
数据二&nbsp; &nbsp; &nbsp; &nbsp; : 美国 | APNIC&amp;CloudFlare公共DNS服务器<br />
<br />
数据三&nbsp; &nbsp; &nbsp; &nbsp; : 澳大利亚<br />
<br />
URL&nbsp; &nbsp; &nbsp; &nbsp; : http://www.cip.cc/1.1.1.1

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350236&amp;ptid=758302" target="_blank"><font color="#999999">wcn 发表于 2020-10-25 16:12</font></a></font><br />
curl是服务器ip</blockquote></div><br />
<br />
嗯嗯，所以我想找一个可以带参数(IP)查询的。<br />
已经找到了<img src="static/image/smiley/yct/011.gif" smilieid="33" border="0" alt="" />

纳闷你找接口和 curl&nbsp;&nbsp;有什么关系

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9350283&amp;ptid=758302" target="_blank"><font color="#999999">william2ct 发表于 2020-10-25 16:22</font></a></font><br />
纳闷你找接口和 curl&nbsp;&nbsp;有什么关系</blockquote></div><br />
有些是返回一堆html的，看得不舒服。<br />
有些是返回IP和地址，这种比较简洁。<br />
我只是让别人知道我是拿什么工具去使用的，从而能找到更好的(更适合这种用法)接口。
