# CF防火墙规则


<i class="pstatus"> 本帖最后由 shvod 于 2020-10-22 20:06 编辑 </i><br />
<br />
只想屏蔽特定国家的IP地址，写成这样可行吗？<br />
<br /><div class="blockcode"><div id="code_M3U"><ol><li>(ip.geoip.country in {&quot;JP&quot; &quot;US&quot; &quot;CA&quot;} and not cf.client.bot) </ol></div><em onclick="copycode($('code_M3U'));">复制代码</em></div><br />
<br />
统统block掉<br />
<br />
有提升空间不的？

直接屏蔽.cn

帮顶，不是很懂<br />
<br />
我是用官方的！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />
