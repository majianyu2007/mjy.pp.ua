# 【大牛来】Win10系统启动时，如何自动跳过“恢复”界面？


给电脑设置了来电自启，如果意外断电的情况下，设备会自动启动。但是遇到有时启动时无法进入系统，卡在“恢复”界面，需要用键鼠配合点击重启才行。<br />
<br />
由于设备距离较远，而且需要人为的配合才能进入桌面，非常的不方便。<br />
<br />
问下大家是否有什么办法，能在意外断电重启时，能顺利进入桌面，跳过必须要手动操作的“恢复”操作？

加UPS电源

修改注册表和组策略！<br />
<br />
具体百度去搜！<br />
<br />
别什么都伸手党！<br />
<br />
<img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" /><img src="static/image/smiley/default/time.gif" smilieid="15" border="0" alt="" />

操作系统内<br />
管理员运行命令行<br />
bcdedit /set {current} recoveryenabled no

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9351197&amp;ptid=758369" target="_blank"><font color="#999999">宣传 发表于 2020-10-25 20:41</font></a></font><br />
操作系统内<br />
管理员运行命令行<br />
bcdedit /set {current} recoveryenabled no</blockquote></div><br />
设置完之后，还是会有一个恢复界面，提示未正常启动。 隔两次异常断电启动后就必然会出现<br />
<br />
不过还是非常感谢老师傅～

加个UPS不香吗？

两三千买一个KVM不香吗<img src="static/image/smiley/yct/010.gif" smilieid="41" border="0" alt="" /><br />
我都是PCIE开机卡
