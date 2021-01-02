# wp 三十万文章搜索功能贼慢，咋整


<i class="pstatus"> 本帖最后由 爱吃醋的醋醋 于 2020-11-25 10:10 编辑 </i><br />
<br />
有点后悔了用wp了<br />
<br />
叁拾万的文章而已<br />
<br />
搜索一个词能卡TM 几十秒<br />
<br />
Intel(R) Xeon(R) CPU E5-2620 v2 <a href="https://www.hostloc.com/home.php?mod=space&amp;uid=175" target="_blank">@</a> 2.10GH<br />
<br />
10G内存<br />
<br />
硬盘 io 400M <br />
<br />
咋优化能变快？<br />
<br />
w3c缓存插件<br />
<br />
全部开了 memcached的缓存

搜索用百度。自己的禁用了。

有机器配置有关吗？还好我才一万多点 <img src="static/image/smiley/default/biggrin.gif" smilieid="3" border="0" alt="" />

大数据换cms

<i class="pstatus"> 本帖最后由 imslc 于 2020-11-25 10:14 编辑 </i><br />
<br />
使用主频3.5以上的cpu,硬盘IO达到1000M/s.<br />
<br />
对于数据库搜索而言,高主频的影响远远大于多核心,另外就是硬盘io越快,体验越好.

采集用WP也是大神， 坐等解决方案。。。。不是还有个redis吗

自建ES搜索，但是我建了不知道怎么和主题融合，感觉开了和没开差不多

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9513407&amp;ptid=771085" target="_blank"><font color="#999999">栉风沐雨 发表于 2020-11-25 10:20</font></a></font><br />
采集用WP也是大神， 坐等解决方案。。。。不是还有个redis吗</blockquote></div><br />
哈哈哈，当初没想到测试站居然能来这么多ip，就一直采下去了

听大佬说用DZ速度快

有90万文章，一点事没有，上Elasticpress
