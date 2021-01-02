# VMware下能安装docker吗，以解决


<i class="pstatus"> 本帖最后由 qxwo 于 2020-10-24 15:50 编辑 </i><br />
<br />
root@debian:~# curl -fsSL https://get.docker.com | bash -s docker --mirror Aliyun<br />
# Executing docker install script, commit: 26ff363bcf3b3f5a00498ac43694bf1c7d9ce16c<br />
+ sh -c 'apt-get update -qq &gt;/dev/null'<br />
+ sh -c 'DEBIAN_FRONTEND=noninteractive apt-get install -y -qq apt-transport-https ca-certificates curl gnupg &gt;/dev/null'<br />
<br />
用脚本安装卡在这里。<br />
<font color="Red">好像是网速慢。。。。。。</font>

这个是正常的回显，等一会就行<br />
<br />


目测是网络问题、还在下载包吧

对了，国内的机器建议用这个安装，快一些<br />
<br />
网址：https://get.daocloud.io/<br />
<br />
curl -sSL https://get.daocloud.io/docker | sh
