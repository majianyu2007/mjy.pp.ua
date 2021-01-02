# travis-ci 255退出


<i class="pstatus"> 本帖最后由 家有自己自温暖 于 2020-11-5 18:07 编辑 </i><br />
<br />
<img id="aimg_CEu95" onclick="zoom(this, this.src, 0, 0, 0)" class="zoom" src="https://imgloc.com/images/2020/11/05/rmXk.png" onmouseover="img_onmouseoverfunc(this)" onload="thumbImg(this)" border="0" alt="" /><br />
<br />
请问大佬这个错误为什么会出现呐？<br />
<br />
我就是使用travis-ci构建HUGO的时候发生的<br />
<br /><div class="blockcode"><div id="code_sYM"><ol><li>language: go<br /><li><br /><li>go:<br /><li>&nbsp;&nbsp;- &quot;1.8&quot;&nbsp;&nbsp;# 指定Golang 1.8<br /><li><br /><li># Specify which branches to build using a safelist<br /><li># 分支白名单限制: 只有hugo分支的提交才会触发构建<br /><li>branches:<br /><li>&nbsp;&nbsp;only:<br /><li>&nbsp; &nbsp; - main <br /><li><br /><li>env:<br /><li>&nbsp;&nbsp;global:<br /><li>&nbsp; &nbsp; # 设定 Github Pages 环境变量<br /><li>&nbsp; &nbsp; - GH_REF: github.com/xxx/xxx<br /><li><br /><li>install:&nbsp;&nbsp;# 安装依赖<br /><li>&nbsp;&nbsp;# 安装 hugo （version: v0.66.0）<br /><li>&nbsp;&nbsp;- wget https://github.com/gohugoio/hugo/releases/download/v0.66.0/hugo_extended_0.66.0_Linux-64bit.deb<br /><li>&nbsp;&nbsp;- sudo dpkg -i hugo*.deb<br /><li>&nbsp; &nbsp; # 安装主题<br /><li>&nbsp;&nbsp;- git clone https://github.com/xxx/xxx.git<br /><li><br /><li>script:<br /><li>&nbsp;&nbsp;- hugo&nbsp;&nbsp;# 生成网站<br /><li><br /><li>deploy:<br /><li>&nbsp;&nbsp;provider: pages&nbsp;&nbsp;# 部署到 Github Pages<br /><li>&nbsp;&nbsp;skip_cleanup: true&nbsp;&nbsp;# 必须为 true ，否则 Travis 会删除在构建期间创建的所有文件（即删除了要上传的文件）<br /><li>&nbsp;&nbsp;local_dir: public&nbsp;&nbsp;# 被推送到 GitHub Pages 的目录，可以指定为当前目录的绝对路径或相对路径<br /><li>&nbsp;&nbsp;on:<br /><li>&nbsp; &nbsp; branch: main&nbsp;&nbsp;# 博客源码所在分支<br /><li>&nbsp;&nbsp;target_branch: gh-pages&nbsp;&nbsp;# 将 local-dir 强制推送到哪个分支（自定义，名称不能与源代码分支名相同），默认为 gh-pages<br /><li>&nbsp;&nbsp;token: $GITHUB_TOKEN<br /><li>&nbsp;&nbsp;strategy: git<br /><li>&nbsp;&nbsp;keep_history: true&nbsp;&nbsp;# 保持 target-branch 分支的提交记录<br /><li>&nbsp;&nbsp;<br /><li></ol></div><em onclick="copycode($('code_sYM'));">复制代码</em></div>

帮顶，技术大佬帮回答吧！<br />
<br />
<img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" /><img src="static/image/smiley/default/lol.gif" smilieid="12" border="0" alt="" />

branch一般是master 看看改完能不能build
