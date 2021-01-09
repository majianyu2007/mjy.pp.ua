# LuManager网站服务器管理面板已开源，可用于商用


<i class="pstatus"> 本帖最后由 zhoumo310 于 2020-10-26 11:24 编辑 </i><br />
<br />
LuManager估计HOC里很多人都没听过。LuManager是基于FreeBSD、Zijidelu、Debian、Centos、Ubuntu等等的面板，国内好像仅此一个可以同时支持Linux和Unix。如果MJJ们有兴趣研究这个面板，或者有开发能力，可以对LuManager面板开发定制，开源免费（基于Apache2开源协议），可用于商用。<br />
<br />
<br />
<font color="Red"><strong>下载地址：</strong><br />
https://wws.lanzous.com/b01bt4vmj<br />
密码:dzh9<br />
解压密码：urlos.com<br />
</font><br />
<br />
LuManager的作者后面成立了公司并开发了全新的URLOS面板，不会开发的小白可以直接选择URLOS这个面板。<br />
<br />
现在URLOS双11促销，标准版终身授权也只要11.11元，活动看这里<br />
<br />
<strong><font color="Blue">https://www.hostloc.com/thread-758311-1-1.html</font></strong><br />
<br />


<br />
<br />
#-------- Nginx和Tengine自由切换<br />
Tengine是由淘宝技术团队开发的Web服务器，Tengine基于Nginx，针对大流量网站需求增加了很多功能特性和性能优化（taobao.com就用它！）。<br />
<br />
#-------- Nginx(Tengine)与Apache自由切换<br />
每个网站都可以自由选择以下三种模式：1.完全使用Nginx，2.完全使用Apache，3.仅PHP用Apache处理（即前台Nginx，后台Apache）。并且可以选择是否使用cgi处理PHP，杜绝502错误。<br />
<br />
#-------- 傻瓜化挂载硬盘<br />
在LUM2.0出现之后，您只需要知道怎么插硬盘线就行了，别的事都交给LUM吧！阿里云，盛大云的数据库硬盘可以挂吗？哈哈，当然的，简直易如反掌，您不是在做梦！<br />
<br />
#-------- 智能优化<br />
LUM可以根据硬件的性能智能优化系统，您只需打开智能优化开关即可，完全没有必要花大量的时间学习如何优化！还可以直接修改php,mysql的参数，如mysql连接数，php上传文件大小等。<br />
<br />
#-------- 增加了API接口<br />
开发者可以开发主控端了！什么卖空间啦，FTP啦，都不在话下。不限制主控端的开发语言，理论上，只要能提交post数据，并**json数据的语言便可。<br />
<br />
#-------- 互相操控<br />
如果您有1000台机装有LUM，要记账号，密码，还得不停切换...管理起来是不是特别麻烦？现在好了，只需要在其中一台LUM中录入其它999个节点的API接口密码（装有LUM的服务器，便可以称为节点），便可以管理其它机器了，可以往节点服务器上添加网站，重启，关机...跟管理本机一样操作，连界面都不变，只多出一个提示：您正在操控IP为****的节点服务器，爽得要死！<br />
<br />
#-------- 杜绝病毒与木马，安全有保障<br />
LUM可以将网站“上锁”，就算网站程序有漏洞，也不会被挂木马或中病毒。至于跨站攻击，我们在很久很久以前就已经解决了...听说LUM还没有出现过漏洞？对头，相信我们，没错滴！<br />
<br />
#-------- 禁止访客IP<br />
当发现某客户端IP的访客过多时，可以在LUM后台禁止访客IP<br />
<br />
#-------- 清理垃圾<br />
相信没有几个人懂得Linux/Unix系统里所有文件的作用，而LUM可以将那些垃圾文件找出来！至于你信不信...哦，至于删除还是不删除，由你！<br />
<br />
#-------- 半小时内即可装好服务器环境<br />
如果您使用的Reh系列操作系统（如CentOS，HttpOS等），一般30分钟即可装好服务器环境；如果选择编译安装，一般也不会超过2小时（与机器性能与下载速度有关，但我们还是强烈推荐用编译安装，因为安装过程中会根据硬件环境自动优化）。不管您选择哪一种方式，都可以自动化安装。<br />
<br />
#-------- 邮件告警<br />
当系统发生故障时或进行一些重要的操作时，将发邮件给管理员告警。<br />
<br />
#-------- 服务器资源共享（LUM是非常优秀的虚拟主机控制面板）<br />
LUM支持无限级代理，每个用户都可以创建子用户，并为子用户指定用户组，然后通过用户组控制子用户的权限，就像鸡生蛋，蛋再生鸡和寡蛋...LUM的权限控制可以精确到具体行为，例如可让某用户的网站跨目录访问，是否有重启Nginx的功能等。哦，对了，用户可以在LUM发邮件烦管理员哦！<br />
<br />
#-------- 网站压力测试<br />
想试一下服务器的性能吗？想知道度娘的反应速度如何吗？<br />
<br />
#-------- 同时支持PHP5.2X和PHP5.3X<br />
如果朋友们想使用PHP5.3X，选择Apache即可（选择Nginx就使用PHP5.2）<br />
<br />
#-------- 可以使用PostgreSQL数据库<br />
兄弟姐妹们，如果MySQL宕掉了，LUM是不是就不能用了？以前是，以后，不一定了...只需在LUM后台点点鼠标即可切换成PostgreSQL，LUM的稳定性又一次大大增强<br />
<br />
#-------- CDN静态网站加速<br />
提供静态内容加速功能，让不同地区或线路的用户访问不同的服务器，是下载或镜像网站的解决方案（创建一个镜像网站是几秒钟的事情）。最简单的应用：可以非常轻松实现让电信用户访问电信服务器，联通用户访问联通服务器，老外就访问放在国外的服务器...并且我们即将推出动态网站的加速软件，可以加速discuz,phpwind等动态网站的内容。<br />
<br />
#-------- 在线安装常用软件<br />
可在线安装Discuz/Phpwind/EcShop/EcGroupon/Xweibo/iWeibo/PhpCMS/ECMS等程序，会上网就会建网站！<br />
<br />
#-------- 防止跨站攻击<br />
不论使用的是Apache还是Nginx，都可以防跨站攻击，当服务上的一个网站出现安全问题并不会危及整台服务器上的数据。<br />
<br />
#-------- SSL证书支持<br />
可以用LUM直接生成ssl证书和证书申请文件，生成后马上就可以用（测试站点），任何人都可以创建支持SSL证书的站点，不需再用命令去操作。<br />
<br />
#-------- 301和302转向<br />
可以设置301永久转向和302临时转向。<br />
<br />
#-------- 网站流量限制<br />
可以设置每个访客的最大线程和最大的浏览网页的速度。<br />
<br />
#-------- 同时支持Linux和Unix系统<br />
目前已经支持的系统有FreeBSD（Unix系），Debian，Ubuntu系列（Linux mint, 深度Linux，YLMF Linux，KUbuntu等），Redhat系列（RHEL, CentOS等）...最重要的，LUM不会破坏系统的安全保护机制，请放心使用！<br />
<br />
#-------- 在线下载远程数据<br />
填入远程文件的网址，轻轻一点便可以将远程文件下载，同时支持将整个FTP上的内容下载（搬站是件蛮好玩的事...）<br />
<br />
#-------- 强大的流量统计功能<br />
能统计网站的最近5分钟，10分钟，半小时，3天，7天、10天、180天，本月，本年，昨天等时间段流量。自定义统计时间，支持日志回滚和自动切割，不需担心日志过大的问题。并且可以生成流量统计图表。还可以对单个网站进行流量统计，如果您感觉网站太难找，可以搜索并统计网站的流量。<br />
<br />
#-------- 支持套餐定制<br />
可以对产品（FTP，虚拟主机，数据库）进行集中管理，如增加FTP的下载速度，限制FTP大小，控制FTP、网站、数据库的个数等，接下来还将开发支持限制资源使用的功能。<br />
<br />
#-------- FTP，主机，数据库分离<br />
一个FTP下可以建N个网站，一个网站可以连接任意多个数据库，数据库和网站只相关不相连。一个用户可以有N个FTP，一个FTP下又可以有N个网站。<br />
<br />
#-------- 反向代理<br />
只需填写被代理网址，别的都交给LUM去做，而且可以为代理网站开启静态缓存。<br />
<br />
#-------- 身份验证<br />
可以为网站增加一个访问用户名和密码，只有通过验证的用户才能访问网站。<br />
<br />
#-------- 可选择常用软件的伪静态规则<br />
包括Discuz、PhpWind、ShopEX、Wordpress等常用程序的伪静态规则。<br />
<br />
#-------- Memcached缓存管理<br />
在线启动和关闭Memcached，并可设置所使用的内存大小，连接数，是否开机启动等。<br />
<br />
#-------- 防盗链<br />
不仅可以设置允许链接的域名，还可以设置被盗链时的默认图片。<br />
<br />
#-------- 备份与还原<br />
支持对网站，数据库或者普通文件夹直接打包备份或者解压还原，支持zip, tar.gz, bz2等压缩格式。<br />
<br />
#-------- 操作系统行为控制<br />
支持在后台直接重启，关机，Nginx，Apache，MySQL，Pure-ftpd等软件的重启，重载，关闭等功能。<br />
<br />
#-------- 操作FTP和网站的文件权限互通系统<br />
开通网站后，能过FTP上传程序即可使用，不需改文件权限。通过FTP上传的文件在网站程序中可以编辑或删除，网站生成的文件在FTP中也能编辑或删除。而且可在编辑虚拟主机时一次性将网站所有文件更改成777、775、644等权限。<br />
<br />
#-------- 错误页控制<br />
支持在后台控制403、404、500、501、502错误页<br />
<br />
#-------- FTP和网站目录自由定制<br />
可以将FTP定在/home/以外的分区，支持多个FTP主目录（即可以挂多个硬盘），如/home/ftp2，/home/ftp3。<br />
<br />
从LUM1.1.9至2.0有100多项更新，在此不再赘述。<br />


<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> 这AD有点硬

好多年前lnmp我玩不转就用的撸妹儿

因为你的头像，你的帖子我都不敢在办公室点开<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9352923&amp;ptid=758493" target="_blank"><font color="#999999">boq 发表于 2020-10-26 10:44</font></a></font><br />
因为你的头像，你的帖子我都不敢在办公室点开</blockquote></div><br />

<ignore_js_op>

<img id="aimg_140747" aid="140747" src="static/image/common/none.gif" zoomfile="forum.php?mod=attachment&aid=MTQwNzQ3fDg4MWRhN2NifDE2MDk2MjE3MDF8NDczNDR8NzU4NDkz&noupdate=yes&nothumb=yes" file="forum.php?mod=attachment&aid=MTQwNzQ3fDg4MWRhN2NifDE2MDk2MjE3MDF8NDczNDR8NzU4NDkz&noupdate=yes" class="zoom" onclick="zoom(this, this.src, 0, 0, 0)" width="200" id="aimg_140747" inpost="1" onmouseover="showMenu({'ctrlid':this.id,'pos':'12'})" />

<div class="tip tip_4 aimg_tip" id="aimg_140747_menu" style="position: absolute; display: none" disautofocus="true">
<div class="xs0">
<p><strong>71_avatar_big.jpg</strong> <em class="xg1">(9.36 KB, 下载次数: 0)</em></p>
<p>
<a href="forum.php?mod=attachment&amp;aid=MTQwNzQ3fDg4MWRhN2NifDE2MDk2MjE3MDF8NDczNDR8NzU4NDkz&amp;nothumb=yes" target="_blank">下载附件</a>

</p>

<p class="xg1 y">2020-10-26 10:50 上传</p>

</div>
<div class="tip_horn"></div>
</div>

</ignore_js_op>
<br />
<br />
这样会不会好些<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /> 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9352902&amp;ptid=758493" target="_blank"><font color="#999999">_____________Cc 发表于 2020-10-26 10:41</font></a></font><br />
好多年前lnmp我玩不转就用的撸妹儿</blockquote></div><br />
我用的第一个面板就是这个，后来转用wdcp，用了好几年，然后用amh

换名字啦

楼主解压密码多少？

头像好牛
