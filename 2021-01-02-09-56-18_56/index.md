# EHEH.ORG 新增CN2线路检测


<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376699&amp;ptid=760329" target="_blank"><font color="#999999">Eric.c 发表于 2020-10-30 19:13</font></a></font><br />
估计规则还有不足得地方， 求个规则</blockquote></div><br />
59.43出海线路阿 没有AS号 

帮顶

CN2 GIA的识别，最好是使用除北上广外的节点省份，比如四川成都<br />
<br />
这些地区如果是GIA的链路的话，会在本省互联点进入59.43骨干网，选成都的原因还有一个就是成都不负载周边省份的CN2入口，所以一定不会出现202.97<br />
<br />
至于北上广，GIA也可能会出现202.97那一跳，因为骨干负载高现在什么可能性都有<br />
<br />
GT的话很好辨别，以成都为例，出现202.97一定就是GT<br />
<br />
还有就是CERA这种去163回GIA的，最好就是用MTR测试丢包率综合判断

不能访问。。。为啥。因为我在Q内？

可以，hin好用<img src="static/image/smiley/yct/019.gif" smilieid="49" border="0" alt="" />

<i class="pstatus"> 本帖最后由 Eric.c 于 2020-10-30 22:00 编辑 </i><br />
<div class="quote"><blockquote><font color="#999999">我y零kk 发表于 2020-10-30 19:56</font><br />
<font color="#999999">CN2 GIA的识别，最好是使用除北上广外的节点省份，比如四川成都<br />
<br />
这些地区如果是GIA的链路的话，会在本省互 ...</font></blockquote></div><br />
<br />
感谢感谢，周末挪到成都去。<br />
服务端到国内的也会有相应的测试提供<br />


<div class="quote"><blockquote><font color="#999999">Hedy 发表于 2020-10-30 18:49</font><br />
<font color="#999999">把加速类型也加进去啊</font></blockquote></div><br />
这是什么？？？

<div class="quote"><blockquote><font color="#999999">铅笔 发表于 2020-10-30 19:24</font><br />
<font color="#999999">59.43出海线路阿 没有AS号</font></blockquote></div><br />
不是很明白，来个指点&nbsp; &nbsp; 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9378091&amp;ptid=760329" target="_blank"><font color="#999999">Eric.c 发表于 2020-10-30 21:56</font></a></font><br />
感谢感谢，周末挪到成都去。<br />
服务端到国内的也会有相应的测试提供</blockquote></div><br />
如果服务端测那就简单了，找个成都电信的DNS测过去，比如61.139.2.69<br />
<br />
回程出现202.97就是GT，肯定在广州，不出现就是GIA了<br />
<br />
其实除了北美电信都没区分GT和GIA这种，甲骨文和阿里轻量都是故意屏蔽了4809的路由，导致去程收不到CN2路由，回程又没有其他的线路，送去4809因为缺路由就变GT了

<div class="quote"><blockquote><font color="#999999">我y零kk 发表于 2020-10-30 22:18</font><br />
<font color="#999999">如果服务端测那就简单了，找个成都电信的DNS测过去，比如61.139.2.69<br />
<br />
回程出现202.97就是GT，肯定在广州 ...</font></blockquote></div><br />
普通线路怎么区分呢
