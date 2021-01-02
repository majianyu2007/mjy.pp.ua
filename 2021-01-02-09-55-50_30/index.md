# 如果网站有证书，反代要怎设置？


用nginx 后端要配置证书吗？还是用前端同样的证书。搞不明白

一样的即可

当然是一样都要配置证书啊

用同一个证书就可以了，反向代理看你自己要怎么优化

一样的亲。。。。<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

用自己的证书

<i class="pstatus"> 本帖最后由 havoc06 于 2020-11-4 00:12 编辑 </i><br />
<br />
反代如果被反代站点也开了https的话要注意设置sni<br />
proxy_ssl_name $host;<br />
proxy_ssl_server_name on;<br />
可以参考一下这个 ：&nbsp;&nbsp;<a href="https://notesail.com/posts/typecho-reverse-proxy.html" target="_blank">https://notesail.com/posts/typecho-reverse-proxy.html</a><br />


反代端必须有证书&nbsp;&nbsp;后端有没有无所谓 只要让前端能访问&nbsp;&nbsp;跟CDN设置一个道理

两种方式<br />
1. 4层，tcp转发。直接转发数据到后端，后端配置证书（用前端域的证书）<br />
2. 7层，http代理。前端配置证书，后端走http/https都行，看自己。前后端配置各自的证书。
