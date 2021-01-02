# AWS cdn 添加域名的时候报错


<i class="pstatus"> 本帖最后由 zhongziso 于 2020-11-4 19:04 编辑 </i><br />
<br />
买的aws全区号<br />
<br />
添加域名的时候，创建资源分配。报错了。有大佬知道是什么原因呢？<br /><div class="blockcode"><div id="code_Rv3"><ol><li>com.amazonaws.services.cloudfront.model.AccessDeniedException: Your account must be verified before you can add new CloudFront resources. To verify your account, please contact AWS Support (https://console.aws.amazon.com/support/home#/) and include this error message. (Service: AmazonCloudFront; Status Code: 403; Error Code: AccessDenied; Request ID: 5152bc48-84ee-457e-8782-5fd9645396f8; Proxy: null)</ol></div><em onclick="copycode($('code_Rv3'));">复制代码</em></div><br />
<br />
<img id="aimg_bh16z" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://i.loli.net/2020/11/04/ivAfakpT3HGxRLu.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
解决方案：<br />
<br />
https://forums.aws.amazon.com/thread.jspa?threadID=307967

求指导

 Your account must be verified before you can add new CloudFront resources. 

<div class="quote"><blockquote><font size="2"><a href="https://www.hostloc.com/forum.php?mod=redirect&amp;goto=findpost&amp;pid=9402940&amp;ptid=762444" target="_blank"><font color="#999999">PHP是最好的语言 发表于 2020-11-4 18:28</font></a></font><br />
Your account must be verified before you can add new CloudFront resources.</blockquote></div><br />
不知道怎么验证

To verify your account, please contact AWS Support (https://console.aws.amazon.com/support/home#/) and include this error message. (Service: AmazonCloudFront; Status Code: 403; Error Code: AccessDenied; Request ID: 5152bc48-84ee-457e-8782-5fd9645396f8; Proxy: null)

你不是要申请工单吗？你这是通过了吗？
