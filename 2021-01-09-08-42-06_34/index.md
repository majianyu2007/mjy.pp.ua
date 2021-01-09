# 有没有大佬使用过verynginx的吗？


为毛我配置写不进去？<br />
<br />
添加用户刷新就没了，而且原始账户也删除不了。nginx配置也无法生效。<br />
<br />
<font size="2">这是什么原因？？？？？</font><br />
<img id="aimg_MtL80" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="225" src="https://i.w3tt.com/images/o7vdv.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<img id="aimg_om6ZC" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="600" height="225" src="https://i.w3tt.com/images/o7ZvY.png" onmouseover="img_onmouseoverfunc(this)" onclick="zoom(this)" style="cursor:pointer" border="0" alt="" /><br />
<img id="aimg_O9z1Q" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" width="489" height="261" src="https://i.w3tt.com/images/o7KUU.png" border="0" alt="" />

不要加到 listen 888<br />
建议先学《nginx各层配置指南》、《宝塔 phpMyAdmin 实现方式》<img id="aimg_V7l77" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376964&amp;ptid=760363" target="_blank"><font color="#999999">iks 发表于 2020-10-30 19:55</font></a></font><br />
不要加到 listen 888<br />
建议先学《nginx各层配置指南》、《宝塔 phpMyAdmin 实现方式》 ...</blockquote></div><br />
之前是添加到下面的，但是也没用，所以我按着它实例添加了一次，还是没用！<img id="aimg_qZu6w" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.w3tt.com/images/o7gaq.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 iks 于 2020-10-30 20:04 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9376996&amp;ptid=760363" target="_blank"><font color="#999999">peng123 发表于 2020-10-30 20:01</font></a></font><br />
之前是添加到下面的，但是也没用，所以我按着它实例添加了一次，还是没用！ ...</blockquote></div><br />
<br />
server段conf添加到你需要添加的网站的server里去（/www/server/panel/vhost/nginx或网站-配置文件），不是随意添加到哪个server里就行的<img id="aimg_KxyDz" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

仔细看项目文档，你遇到的这个问题里边提到的有

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9377009&amp;ptid=760363" target="_blank"><font color="#999999">iks 发表于 2020-10-30 20:03</font></a></font><br />
server段conf添加到你需要添加的网站的server里去（/www/server/panel/vhost/nginx或网站-配置文件），不 ...</blockquote></div><br />
还是没作用啊，添加配置后刷新还是没了！<br />
<br />
<img id="aimg_RX0Xb" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.w3tt.com/images/o7pEr.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<img id="aimg_mnV2N" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.w3tt.com/images/o7mNc.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />


用过 难用。放弃了。还是宝塔nginx防火墙好用。

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9377107&amp;ptid=760363" target="_blank"><font color="#999999">peng123 发表于 2020-10-30 20:20</font></a></font><br />
还是没作用啊，添加配置后刷新还是没了！</blockquote></div><br />
<br />
include /opt/verynginx/verynginx/nginx_conf/in_external.conf;放在 http 配置块外部<img id="aimg_HtykM" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 iks 于 2020-10-30 20:27 编辑 </i><br />
<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9377107&amp;ptid=760363" target="_blank"><font color="#999999">peng123 发表于 2020-10-30 20:20</font></a></font><br />
还是没作用啊，添加配置后刷新还是没了！</blockquote></div><br />
<strong>server段放对了</strong><br /><div class="blockcode"><div id="code_lbo"><ol><li>user&nbsp;&nbsp;www www;<br /><li>worker_processes auto;<br /><li>error_log&nbsp;&nbsp;/www/wwwlogs/nginx_error.log&nbsp;&nbsp;crit;<br /><li>pid&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;/www/server/nginx/logs/nginx.pid;<br /><li>worker_rlimit_nofile 51200;<br /><li><br /><li>events<br /><li>&nbsp; &nbsp; {<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;use epoll;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;worker_connections 51200;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;multi_accept on;<br /><li>&nbsp; &nbsp; }<br /><li><br /><li>include /opt/verynginx/verynginx/nginx_conf/in_external.conf;<br /><li><br /><li>http<br /><li>&nbsp; &nbsp; {<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; include /opt/verynginx/verynginx/nginx_conf/in_http_block.conf;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;include&nbsp; &nbsp;&nbsp; &nbsp; mime.types;<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; #include luawaf.conf;<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; include proxy.conf;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;default_type&nbsp;&nbsp;application/octet-stream;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;server_names_hash_bucket_size 512;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;client_header_buffer_size 32k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;large_client_header_buffers 4 32k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;client_max_body_size 50m;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;sendfile&nbsp; &nbsp;on;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;tcp_nopush on;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;keepalive_timeout 60;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;tcp_nodelay on;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_connect_timeout 300;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_send_timeout 300;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_read_timeout 300;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_buffer_size 64k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_buffers 4 64k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_busy_buffers_size 128k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;fastcgi_temp_file_write_size 256k;<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; fastcgi_intercept_errors on;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip on;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_min_length&nbsp;&nbsp;1k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_buffers&nbsp; &nbsp;&nbsp;&nbsp;4 16k;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_http_version 1.1;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_comp_level 2;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_types&nbsp; &nbsp;&nbsp;&nbsp;text/plain application/javascript application/x-javascript text/javascript text/css application/xml;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_vary on;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_proxied&nbsp; &nbsp;expired no-cache no-store private auth;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;gzip_disable&nbsp; &nbsp;&quot;MSIE [1-6]\.&quot;;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;limit_conn_zone $binary_remote_addr zone=perip:10m;<br /><li>&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; limit_conn_zone $server_name zone=perserver:10m;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;server_tokens off;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;access_log off;<br /><li><br /><li>server<br /><li>&nbsp; &nbsp; {<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;listen 888;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;server_name phpmyadmin;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;index index.html index.htm index.php;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;root&nbsp;&nbsp;/www/server/phpmyadmin;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;location ~ /tmp/ {<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; return 403;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;}<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;#error_page&nbsp; &nbsp;404&nbsp; &nbsp;/404.html;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;include enable-php.conf;<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;location ~ .*\.(gif|jpg|jpeg|png|bmp|swf)$<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;{<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;expires&nbsp; &nbsp;&nbsp; &nbsp;30d;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;}<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;location ~ .*\.(js|css)?$<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;{<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;expires&nbsp; &nbsp;&nbsp; &nbsp;12h;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;}<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;location ~ /\.<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;{<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp;deny all;<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;}<br /><li><br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;access_log&nbsp;&nbsp;/www/wwwlogs/access.log;<br /><li>&nbsp; &nbsp; }<br /><li><br /><li>include /www/server/panel/vhost/nginx/*.conf;<br /><li>}<br /><li></ol></div><em onclick="copycode($('code_lbo'));">复制代码</em></div><br />
注意第<strong>14</strong>行和第<strong>18</strong>行<img id="aimg_xrI70" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9377142&amp;ptid=760363" target="_blank"><font color="#999999">iks 发表于 2020-10-30 20:26</font></a></font><br />
注意第14行和第18行</blockquote></div><br />
可以了。谢谢大佬。用户名以及网站配置都能行了！~<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />
