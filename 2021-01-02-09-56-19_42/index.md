# 需要请求头验证的代理怎么全局使用？


<br />
<br />
假如这是一个Http代理ip<br />
<br />
1.1.1.1:8080<br />
<br />
需要一个请求头作为验证 【cf: cf】<br />
<br />
<br />
比如在python下的requests，可以自定义Headers<br />
<br />
<br />
那么，有没有什么程序可以将其作为全局代理呢？(Linux下)<br />
<br />
<br />
我知道以前那些免流的程序，tiny haproxy之类的就可以（手机上的）<br />
<br />
<br />
然后haproxy好像就可以github.com/haproxy/haproxy<br />
<br />
<br />
这是大概一个反向代理程序？可以修改请求头<br />
<br />
<br />
不过不知道怎么配置，好像在loc里多是用于端口转发<br />
<br />

