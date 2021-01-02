# 反代十倍流量  高价求反代解决方案


同14楼说的，nginx配置要修改下，14楼大佬不接活我接 500块搞定<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><br />
我有个服务器也反代了几个视频，也是发现了类似问题，后面解决了

<div class="quote"><blockquote><font color="#999999">mbfo 发表于 2020-11-5 04:11</font><br />
<font color="#999999">同14楼说的，nginx配置要修改下，14楼大佬不接活我接 500块搞定<br />
我有个服务器也反代了几个视频，也是发 ...</font></blockquote></div><br />
你q发给我 我晚点回去联系你

<div class="quote"><blockquote><font color="#999999">2019年 发表于 2020-11-4 18:27</font><br />
<font color="#999999">刚设置0卡成狗</font></blockquote></div><br />
我这边0正常，可能我视频文件都比较大 10-30g那种

<div class="quote"><blockquote><font color="#999999">BWH 发表于 2020-11-5 10:07</font><br />
<font color="#999999">我这边0正常，可能我视频文件都比较大 10-30g那种</font></blockquote></div><br />
后来发现不卡了，不过入的流量还是超大，你的入站流量正常吗，我视频大概200m

<div class="quote"><blockquote><font color="#999999">2019年 发表于 2020-11-5 10:09</font><br />
<font color="#999999">后来发现不卡了，不过入的流量还是超大，你的入站流量正常吗，我视频大概200m ...</font></blockquote></div><br />
我的正常，上下基本一致，或者你可以试试ngx_http_slice_module切片模块

<div class="quote"><blockquote><font color="#999999">mbfo 发表于 2020-11-5 04:11</font><br />
<font color="#999999">同14楼说的，nginx配置要修改下，14楼大佬不接活我接 500块搞定<br />
我有个服务器也反代了几个视频，也是发 ...</font></blockquote></div><br />
你说的方法不是把视频缓存吧，你的才几个视频可以缓存，我的太多了，空间不够
