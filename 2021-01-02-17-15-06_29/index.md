# 各位MJJ有没有什么优化数据库的方法


RT.<br />
目前使用MySQL 5.6<br />
一张表里面大概7亿条数据 34GB<br />
现在select语句执行慢的要死<br />
各位有没有什么优化查询速度的方法<img src="static/image/smiley/yct/022.gif" smilieid="42" border="0" alt="" /> <br />
<br />
数据库引擎：InnoDB

redis 做缓存<br />
主要还是看你是读多 还是 写多 

数据有点多啊、可以用elasticsearch索引下、专门用于搜索

分表

索引缓存做内存表<br />
<br />
<img id="aimg_Mv6Wf" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://imgurl.mxdreamx.com/2020/10/20/TOIMG3555c1020074632N.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

屌爆了 切表或者换mysql8看看 还得看查询条件是什么

转存其他数据库吧，或者分表分区。如果数据不需要更改的，更可以更换

七亿分表分裤吧
