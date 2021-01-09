# 请问什么是dns解锁奈非呢？？？是中转吗


我的鸡1G口，如果用别人10M口的dns解锁。 那看奈非的话 会变成10M的速度吗？<br />
速度会受对方解锁鸡影响吗

<i class="pstatus"> 本帖最后由 ymcoming 于 2020-10-26 12:16 编辑 </i><br />
<br />
上面答错了，取决于你的vps和dns解锁服务器，谁弱谁就是瓶颈。<br />
<br />
至于为啥会出现楼主那种奇谈怪论，可能过去netflix是这样的，但现在肯定只会在解锁服务器进行数据传输。<br />
<br />
也就是你的vps自以为访问netflix，实际全部流量转到解锁服务器。奈飞那边也是自认为解锁服务器在看奈飞，根本不知道有第三者。<br />
<br />
做解锁的负担了全部流量的中转。

不会吧，感觉就是一个类似头部请求的意思！<br />
<br />
用于欺骗服务器<br />
<br />
我的理解是这样，不对勿喷！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353204&amp;ptid=758515" target="_blank"><font color="#999999">llmwxt 发表于 2020-10-26 11:30</font></a></font><br />
不会吧，感觉就是一个类似头部请求的意思！<br />
<br />
用于欺骗服务器</blockquote></div><br />
也就是说只是欺骗ip 其它的的还是看自己鸡鸡连接速度是吗

楼主大佬来介绍

其实就是把奈飞反代了，所以速度是会受到影响的

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353215&amp;ptid=758515" target="_blank"><font color="#999999">kkdf 发表于 2020-10-26 11:33</font></a></font><br />
也就是说只是欺骗ip 其它的的还是看自己鸡鸡连接速度是吗</blockquote></div><br />
应该是这样吧，不然为什么收解锁鸡鸡的，都只看IP，不管速度、延迟、丢包等等呢！

并不是，资源部分就走你本地的，验证连接走解锁

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353224&amp;ptid=758515" target="_blank"><font color="#999999">TITAN-LOC 发表于 2020-10-26 11:34</font></a></font><br />
其实就是把奈飞反代了，所以速度是会受到影响的</blockquote></div><br />
就是相当于只选择性中转奈非的流量对吗 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9353242&amp;ptid=758515" target="_blank"><font color="#999999">kkdf 发表于 2020-10-26 11:37</font></a></font><br />
就是相当于只选择性中转奈非的流量对吗</blockquote></div><br />
嗯

说白了就是中继所有的Netflix流量。你的网速自然要受制于源站的网络和流量
