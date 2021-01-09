# pr还有更骚的操作！pr服务器怎么样？pr服务器好用吗？


<i class="pstatus"> 本帖最后由 Stillso 于 2020-10-31 12:05 编辑 </i><br />
<br />
之前发过一个贴说pr这垃圾 偷偷换机房网路大如前 https://www.hostloc.com/thread-747011-1-1.html<br />
<br />
随后听取建议发了工单，然后pr回复<br />
<br />
<font color="Red">Hello,<br />
On checking, the node load is fine and your VPS is responding fine to ping and SSH without any issue. Please have a check and let us know how it goes.<br />
--- 155.94.146.2xx ping statistics ---<br />
12 packets transmitted, 12 received, 0% packet loss, time 11012ms<br />
rtt min/avg/max/mdev = 252.943/254.312/265.579/3.414 ms<br />
Kathir Kumar | Senior Engineer<br />
PacificRack Datacneter | 1-877-420-RACK<br />
Asian Optimized VPS, Hybrid Dedicated Servers &amp; Dedicated Servers<br />
www.pacificrack.com</font><br />
<br />
人家简单ping了下说一切正常。<br />
<br />
<font color="Red">Pinging 155.94.146.2xx with 32 bytes of data:<br />
Reply from 155.94.146.2xx: bytes=32 time=192ms TTL=43<br />
。<br />
。<br />
。<br />
Request timed out.<br />
<br />
Ping statistics for 155.94.146.2xx:<br />
Packets: Sent = 12, Received = 10, Lost = 2 (16% loss),<br />
Approximate round trip times in milli-seconds:<br />
Minimum = 182ms, Maximum = 199ms, Average = 189ms</font><br />
<br />
这是我本地ping的（感觉还能用是吧？），随后我又ping了另外一台机器<br />
<font color="Red">Pinging 198.55.122.2xx with 32 bytes of data:<br />
Request timed out.<br />
Request timed out.<br />
Request timed out.<br />
Request timed out.<br />
<br />
Ping statistics for 198.55.122.2xx:<br />
Packets: Sent = 4, Received = 0, Lost = 4 (100% loss),</font><br />
<br />
看到这当时就炸了，随后也回复给了客服，<br />
客服回复：<br />
<font color="Red">Hello,<br />
<br />
We're doing an abuse check and VLAN split. We'll finish this as soon as possible. After that, these issues will be fixed. We appreciate your patience.<br />
我们正在进行滥用检查和VLAN拆分。我们将尽快完成。之后，这些问题将得到解决。感谢您的耐心配合。<br />
Kathir Kumar | Senior Engineer<br />
PacificRack Datacneter | 1-877-420-RACK<br />
Asian Optimized VPS, Hybrid Dedicated Servers &amp; Dedicated Servers</font><br />
<br />
随后就等了，然后过了两天收到了pr的邮件：<br />
你好，<br />
<br />
您的VPS /服务器IP：198.55.122.205有滥用报告。<br />
<br />
原因：您的VPS /服务器似乎已受到威胁，结果试图攻击/入侵网络中的其他服务器<br />
<br />
采取的措施：为阻止滥用行为以及其他服务器受到攻击或黑客攻击的风险，我们别无选择，只能暂停您的VPS。<br />
<br />
建议的解决方案：在大多数情况下，一旦VPS遭到破坏，可能很难将同一VPS置于正常状态，因此建议完全重新安装，如果您同意完全重新安装，请记住所有您的VPS数据将丢失。<br />
<br />
**<br />
如果有任何重要数据，您需要在重新安装之前先进行备份，请告知我们，以便我们在备份过程中为您提供帮助：<br />
创建新的VPS<br />
在受损的VPS上禁用虚拟公共端口，并仅启用专用虚拟端口。<br />
通过虚拟专用网络将受感染的VPS连接到新的VPS。<br />
您将备份重要数据。<br />
然后，我们将终止您受损的VPS，并更新您的WHMCS服务详细信息以反映新创建的VPS。<br />
**<br />
根据我们的政策，我们要求所有客户在收到滥用通知时做出回应。反复出现的未解决或高优先级问题可能会导致对您的上行链路应用过滤器，在其他更严重的情况下甚至可能导致您的帐户被暂停作为一个整体。<br />
<br />
请在我的签名下面找到详细的报告。<br />
来自198.55.122.2xx的电子邮件滥用报告。<br />
已收到电子邮件：2020年10月27日星期二12:29:41 -0500（CDT）。<br />
IP地址198.55.122.2xx现在已列入黑名单。<br />
以下网址粘贴到浏览器承认：<br />
http://m.USGOabuse.net/_AbuseAck?nBvd2VsbGpiQGxpZ2h0Ymxhc3QubmV0OjIwMjAxMDI3MTIyOTQxMTAyNTk1MDAwMDEyOjE5OC41NS4xMjIuMjA1Ol86Og--<br />
OR<br />
如果上面的网址礼物的问题，请访问：<br />
http://m.USGOabuse.net/_AbuseAck<br />
在那里你会需要输入以下信息：<br />
邮箱：<br />
nBvd2VsbGpiQGxpZ2h0Ymxhc3QubmV0<br />
消息：<br />
jIwMjAxMDI3MTIyOTQxMTAyNTk1MDAwMDEy<br />
来源：<br />
jE5OC41NS4xMjIuMjA1<br />
即使您认为该电子邮件<br />
是合法的，我们也只要求您确认此报告。重复的<br />
关于同一来源的报告未被确认将最终<br />
被列入黑名单。感谢您的合作。<br />
此报告采用滥用情况报告格式（“ ARF”，请参阅RFC5965）。<br />
根据该IETF标准的规定，完整的标题和<br />
文本包含在此电子邮件的message / rfc822部分中。<br />
如果有的话，我们报告的收件人地址（<br />
发送报告的地方）由<br />
abusix.com上的滥用联系数据库提供。Abusix使用的所有滥用联系信息均<br />
来自RIR（ARIN，RIPE，LACNIC，APNIC和AFRNIC）<br />
数据库。如果您想更改或报告无效的滥用<br />
联系方式，请联系相应的RIR。有关<br />
虐待联系人数据库的更多信息，请参见：<br />
https:<br />
//abusix.com/contactdb.html Abusix.com对网站内容或内容不承担任何责任。<br />
<br />
此消息的准确性。<br />
等待你的回复，<br />
<br />
谢谢，<br />
<br />
看到这里现在的我工单都不想回了，之说默默的说三遍 ：<br />
pr服务器怎么样？ pr服务器真尼玛垃圾<br />
pr服务器好用吗？&nbsp;&nbsp;pr服务器真尼玛垃圾<br />
<br />
去年真是被猪油蒙了心上了pr这垃圾车，去尼玛的垃圾公司赶紧倒闭吧！<br />
<br />


发帖前请想一下为什么只有你一个人遇到了这种情况<img src="static/image/smiley/yct/013.gif" smilieid="43" border="0" alt="" />

先说下你是不是弱口令的，没检查到你，不代表你就100%没有错。<br />
<br />
要是弱口令，其实你也是网络烂的帮凶，当然他们不做检查不把问题机子关停是他们的错

辣鸡PR，这还是最早的3折鸡，我都怀疑故意劣化赶人下车<br />
<img id="aimg_JPnYj" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/10/31/xEUDC9LoGfnwpVb.jpg" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

是不是用了弱密码

<div class="quote"><blockquote><font color="#999999">Stillso 发表于 2020-10-30 22:59</font><br />
<font color="#999999">是真的垃圾，我都为我之前推过pr的aff感到耻辱，我做梦想到几十个网友被我坑了，还有个直接买了三年就整 ...</font></blockquote></div><br />
我猜你做梦都会笑到呛着

我也不用看了<br />
<br />
就直接结论：<br />
<br />
<font color="Red"><strong>PR就是垃圾</strong>！</font>

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378619&amp;ptid=760415" target="_blank"><font color="#999999">埃隆·马斯克 发表于 2020-10-30 22:53</font></a></font><br />
是不是用了弱密码</blockquote></div><br />
关键是如果真滥用了是不是早就该发这个邮件了？<br />
为什么等我发工单后才发邮件？<br />
你品

开心小站长一直在loc抹**，但没卵用，一波未平息，又一波更大的浪。

垃圾用户警告

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378633&amp;ptid=760415" target="_blank"><font color="#999999">nat.ee 发表于 2020-10-30 22:55</font></a></font><br />
开心小站长一直在loc抹**，但没卵用，一波未平息，又一波更大的浪。</blockquote></div><br />
是真的垃圾，我都为我之前推过pr的aff感到耻辱，我做梦想到几十个网友被我坑了，还有个直接买了三年就整宿整宿睡不着...

用新面板重装试试吧。我重装之前装个内核不到两分钟必关机，重装之后使劲折腾了半小时也没关机，不懂它家的逻辑。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378648&amp;ptid=760415" target="_blank"><font color="#999999">witcat 发表于 2020-10-30 23:00</font></a></font><br />
用新面板重装试试吧。我重装之前装个内核不到两分钟必关机，重装之后使劲折腾了半小时也没关机，不懂它家的 ...</blockquote></div><br />
没必要折腾了这玩意，太垃圾，就算你搞好了，长时间不看又给你办了
