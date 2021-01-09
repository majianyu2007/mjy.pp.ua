# 现在使用的漫画转webp方法，还有啥高效点的吗


<br />
<br />
现在把漫画全部从 jpg 和png 变为了 webp<br />
<br />
可以降低体积和带宽使用率<br />
<br />
目前是火车头采集到的图片，在win下直接使用 格式工厂对所有图片转成了 webp <br />
<br />
然后在sql里面批量换掉 文件格式<br />
<br />
有没有mjj给出比这个方法更加有效率的<br />
<br />
<br />
漫画图片现在的大小&nbsp;&nbsp;3T

进来学习<img id="aimg_CsbXa" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

学习一下

https://github.com/Mogeko/fast2webp<br />
<br />
虽然两年没用维护了，但是用起来没啥问题

进来学习

用这个啊https://github.com/webp-sh/webp_server_go，什么都不用修改

<i class="pstatus"> 本帖最后由 百元大户 于 2020-11-1 12:14 编辑 </i><br />
<br />
webp的编码速度本来就比较慢，快也快不到哪去<br />
还有就是压缩参数的选择问题，用格式工厂这样的过于粗暴了<br />
鄙人之前处理写真原图时写过一个工具，能自动精准设置每一张图的压缩参数<br />
但是算法是针对单张18M左右的高质量大图设计的，大概在你的场景下不适用<br />
鄙人推荐你花一下午时间用自己最擅长的语言写一个最适合自己使用场景的工具<br />
甚至可以再多花点时间把采集上传，sql替换之类的功能全部集成进去

腾讯Cdn自动转换？
