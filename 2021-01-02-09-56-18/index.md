# 大佬们，我这北岸该怎么救


【阿里云】尊敬的用户：经检查您的北岸号粤ICP备号-1下有网站未指向阿里云国内节点（不含香港）服务器且无访问记录 ，请您在3个工作日内进行修改，若规定时间后修改不合格，我们将删除网站北岸接入信息。您的北岸号可能会被注销，网站访问可能受到影响。详情请您查收邮件！<br />
<br />
<br />
今天来短信了<br />
<br />
www跟@是解析给腾讯云香港了<br />
oss静态了一个页面，绑定了二级域名，用阿里云监控定期访问，还是来短信了，我该怎么保住这个北岸

接入

<div class="quote"><blockquote><font color="#999999">庞先生呀 发表于 2020-11-13 19:55</font><br />
<font color="#999999">接入</font></blockquote></div><br />
是在阿里云北岸的

绑定个子域到国内OSS上，OSS里丢个图片啥的小文件，然后随便弄个监控或者宝塔的计划任务，偶尔访问一下这个小文件就行了。<br />
<br />
主要是要产生流量记录

<div class="quote"><blockquote><font color="#999999">aumfoo 发表于 2020-11-13 19:59</font><br />
<font color="#999999">绑定个子域到国内OSS上，OSS里丢个图片啥的小文件，然后随便弄个监控或者宝塔的计划任务，偶尔访问一下这个 ...</font></blockquote></div><br />
已经这样做了，还是来短信了，搞得我不知所措了

应该是

你需要主域名解析阿里云大陆主机 

应该是www和@必须解析到阿里云国内，子域名可以不是，亲测半年稳定

太麻烦了！<img id="aimg_S31aA" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://cdn.jsdelivr.net/gh/hishis/forum-master/public/images/patch.gif" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" />

<i class="pstatus"> 本帖最后由 ABCHINA 于 2020-11-13 20:12 编辑 </i><br />
<br />
北岸的时候主域名就不要填xxx.com和www.xxx.com<br />
北岸主站为xxx.xxx.com指向阿里云oss就行，我就这么干的，www和@现在用的腾讯
