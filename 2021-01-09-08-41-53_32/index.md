# 问个 openLiteSpeed 的问题


<i class="pstatus"> 本帖最后由 dtone 于 2020-10-29 12:35 编辑 </i><br />
<br />
这里大佬多， openLiteSpeed 配置PHP的问题<br />
<br />
用apt-get install lsphp56-sqlite<br />
 <br />
安装typecho 无法选用 sqlite<br />
<br />
不知道怎么配置； 不知道哪位大佬遇到过没<br />
 <br />
apt search lsphp56 也没看到pdo之类的。 <br /><div class="blockcode"><div id="code_Fcv"><ol><li>lsphp54-dev/jessie 5.4.45-1+jessie amd64<br /><li>&nbsp;&nbsp;Files for LSPHP56 module development<br /><li><br /><li>lsphp55-dev/jessie 5.5.38-1+jessie amd64<br /><li>&nbsp;&nbsp;Files for LSPHP56 module development<br /><li><br /><li>lsphp56/jessie,now 5.6.40-13+jessie amd64 [installed]<br /><li>&nbsp;&nbsp;server-side, HTML-embedded scripting language (LSAPI binary)<br /><li><br /><li>lsphp56-curl/jessie,now 5.6.40-13+jessie amd64 [installed]<br /><li>&nbsp;&nbsp;CURL module for lsphp56<br /><li><br /><li>lsphp56-dbg/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;Debug symbols for LSPHP56<br /><li><br /><li>lsphp56-dev/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;Files for LSPHP56 module development<br /><li><br /><li>lsphp56-enchant/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;Enchant module for lsphp56<br /><li><br /><li>lsphp56-gd/jessie,now 5.6.40-13+jessie amd64 [installed]<br /><li>&nbsp;&nbsp;GD module for lsphp56<br /><li><br /><li>lsphp56-gmp/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;GMP module for lsphp56<br /><li><br /><li>lsphp56-imap/jessie,now 5.6.40-13+jessie amd64 [installed]<br /><li>&nbsp;&nbsp;IMAP module for lsphp56<br /><li><br /><li>lsphp56-intl/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;internationalisation module for php5<br /><li><br /><li>lsphp56-ldap/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;LDAP module for lsphp56<br /><li><br /><li>lsphp56-mcrypt/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;MCrypt module for lsphp56<br /><li><br /><li>lsphp56-mysql/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;MySQL module for lsphp56<br /><li><br /><li>lsphp56-odbc/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;ODBC module for lsphp56<br /><li><br /><li>lsphp56-pgsql/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;PostgreSQL module for lsphp56<br /><li><br /><li>lsphp56-pspell/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;pspell module for lsphp56<br /><li><br /><li>lsphp56-recode/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;recode module for lsphp56<br /><li><br /><li>lsphp56-snmp/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;SNMP module for lsphp56<br /><li><br /><li>lsphp56-sqlite/jessie,now 5.6.40-13+jessie amd64 [installed]<br /><li>&nbsp;&nbsp;SQLite module for lsphp56<br /><li><br /><li>lsphp56-tidy/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;tidy module for lsphp56<br /><li><br /><li>lsphp56-xmlrpc/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;XML-RPC module for lsphp56<br /><li><br /><li>lsphp56-xsl/jessie 5.6.40-13+jessie amd64<br /><li>&nbsp;&nbsp;XSL module for lsphp56</ol></div><em onclick="copycode($('code_Fcv'));">复制代码</em></div><br />
<br />
估计需要编译。。。sqlite3！。。好吧 我放弃了。

apt-get install lsphp56-sqlite3

<i class="pstatus"> 本帖最后由 dtone 于 2020-10-29 11:04 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368200&amp;ptid=759721" target="_blank"><font color="#999999">Fei 发表于 2020-10-29 11:00</font></a></font><br />
apt-get install lsphp56-sqlite3</blockquote></div><br />
<br />
 Unable to locate package lsphp56-sqlite3<br />
没有。。。<br />
<br />
SQLite3 module for LSPHP 要到7.0以后才有 好像<br />


我是直接安装cyberpanel面板自带这些。

https://qing.su&nbsp;&nbsp;@香菇肥牛大佬博客有 你看看

<i class="pstatus"> 本帖最后由 Fei 于 2020-10-29 12:13 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368212&amp;ptid=759721" target="_blank"><font color="#999999">dtone 发表于 2020-10-29 11:02</font></a></font><br />
Unable to locate package lsphp56-sqlite3<br />
没有。。。</blockquote></div><br />
<br />
我用的是php7.4，想当然了。你安装应该是lsphp56-sqlite，<u>记得去掉php.ini注释开启sqlite</u>，然后重启php。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9368611&amp;ptid=759721" target="_blank"><font color="#999999">Fei 发表于 2020-10-29 12:07</font></a></font><br />
我用的是php7.4，想当然了。你安装应该是lsphp56-sqlite，记得去掉php.ini注释开启sqlite，然后重启php。 ...</blockquote></div><br />
<br />
之前检查过，ini大致是sqlite3=路径，我估计 只能编译扩展

ols有typecho缓存插件吗
