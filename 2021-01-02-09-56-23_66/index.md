# 国内的高防cc靠谱吗


网站偶尔被CC&nbsp;&nbsp;看见有些什么说无视cc的<br />
想放国内高防 阿里cdn 攻击回源<br />
这样可行吗

<i class="pstatus"> 本帖最后由 chuanchuanlak 于 2020-11-14 00:00 编辑 </i><br />
<br />
<font size="3"><font color="Blue">我以前的discuz经常被CC, 用了一些, 安全狗付费版、阿里云防护企业版、云锁付费版、百度云加速企业版带CC功能,<br />
<br />
价格从几千到上W一年不等, 但都是垃圾, 级别设低了防不住, 设高了乱拦截, 把蜘蛛、api接口访问、正常用户访问一股的全给提示输验证码拦截了,&nbsp;&nbsp;这样的话攻击者正和的意图, 你的蜘蛛权重收录刷刷的掉, 一大堆正常的功能也被破坏了, 他目的不是正达到了吗?<br />
<br />
所以最后不得已, 只有自己写判断逻辑, <br />
方法是: 把30s内每个访问的IP都计入memcache中, 只计入内存缓存30s, 相同IP只记录一次第二次访问时直接把它的数字加1, 然后判断该IP30s内的访问次数就行了.<br />
<br />
用了该方法后, 目前还没有能攻破的, 当然你同时控制攻击的肉鸡有5000以上的话当我没说.<br />
<br />
<br />
还有提示一下: 安全狗和云锁是彻底的大垃圾, 因为它为了防住, 会把别人HTTP_X_FORWARDED_FOR内设置的假IP也给统统禁止掉, HTTP_X_FORWARDED_FOR这个变量别人访问时是可以随便自定义设置的, 别人专门故意设置成百度360 google蜘蛛IP的话, 你的站收录估计会被拔毛了</font></font><br />
<br />
<br />
<font color="Red">最后总结: 防DDOS只能靠高仿IP, <br />
<br />
要想完美防CC攻击只有自己写判断策略才是靠谱的, 比什么几千几万一年的安全软件好多了 </font>

不懂，这些你需要IDC老板和AFF大佬们来解答！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

国内防CC都是金盾吧？

<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />无视CC和80端口一起说的基本金盾无疑，小厂可能是机房自带金盾，但是443金盾没办法，走他们的防御还不如自己弄策略<br />
无视CC基本不可能，但是有的厂家确实防C有自己的方法，但用金盾的，就。。。。<br />
不是很建议买

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451263&amp;ptid=766429" target="_blank"><font color="#999999">chuanchuanlak 发表于 2020-11-13 23:55</font></a></font><br />
我以前的discuz经常被CC, 用了一些, 安全狗付费版、阿里云防护企业版、云锁付费版、百度云加速企业版带CC功 ...</blockquote></div><br />
谢谢了 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451326&amp;ptid=766429" target="_blank"><font color="#999999">heyechuanmei 发表于 2020-11-14 00:16</font></a></font><br />
无视CC和80端口一起说的基本金盾无疑，小厂可能是机房自带金盾，但是443金盾没办法，走他们的防御还不 ...</blockquote></div><br />
谢谢 那我再想想 

reids写个缓存规则，清洗IP

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451513&amp;ptid=766429" target="_blank"><font color="#999999">xiaohei 发表于 2020-11-14 01:46</font></a></font><br />
reids写个缓存规则，清洗IP</blockquote></div><br />
不太会啊 大佬

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9451514&amp;ptid=766429" target="_blank"><font color="#999999">bigbigboss 发表于 2020-11-14 01:47</font></a></font><br />
不太会啊 大佬</blockquote></div><br />
不会程序很痛苦，只能找现成的解决方案。
