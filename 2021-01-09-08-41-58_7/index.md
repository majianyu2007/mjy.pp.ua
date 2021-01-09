# 【结帖】请大佬一个docker问题


<i class="pstatus"> 本帖最后由 huaxing0211 于 2020-10-29 22:23 编辑 </i><br />
<br />
请大佬一个docker问题：<br />
分别运行了一个php、nginx、mysql容器，可以配置多网站么？<br />
试了下，多网站的话，第二个网站php就不能运行了，提示“No input file specified.” 但运行html是没问题的，php容器必须一个网站配置一个么？<br />
<br />
------------------------<br />
<br />
分别运行了一个php、nginx、mysql容器，可以配置多网站（虚拟主机）。小问题坑死人，折腾1天！<br />


帮顶，不懂<br />
<br />
请docker大佬们看到回答！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

先捋顺了再来提问

一个容器一个网站，用不同的端口
