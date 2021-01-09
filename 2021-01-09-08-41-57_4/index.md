# 求问，aws ec2 香港，哪个IP段，广移直连？


如题，现在aws ec2 香港，还有哪个IP段，广州移动是直连的？<br />
我测试过18.162，18.163，18.166几个ip都绕路，之前18.162是直连的。<br />
<br />
然后我用ec2香港，ping之前坛友公布的cloudfront的广州移动ip，延迟也很高；<br />
连自家的cdn延迟都高的话，那还怎么玩？

不清楚，AWS不撸了！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

答案是使用aws 的 AGA 服务
