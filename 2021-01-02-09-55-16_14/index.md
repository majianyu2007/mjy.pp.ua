# 天翼网盘每日可领一日会员，脚本大佬出动，做个定时可好


坐等大佬。。

<div class="blockcode"><div id="code_Arz"><ol><li><br /><li>name: CI<br /><li><br /><li>on:<br /><li>&nbsp;&nbsp;schedule:<br /><li>&nbsp; &nbsp; - cron: &quot;0 1 * * *&quot;<br /><li>&nbsp;&nbsp;watch:<br /><li>&nbsp; &nbsp; types: [started]<br /><li><br /><li>jobs:<br /><li>&nbsp;&nbsp;build:<br /><li>&nbsp; &nbsp; runs-on: ubuntu-latest<br /><li>&nbsp; &nbsp; steps:<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;- uses: actions/checkout@v2<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;- name: receive<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;run: |<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; curl&nbsp;&nbsp;'https://mkt.21cn.com/mkt/api/user/receive/receive.do?activityId=10520&amp;uxChannel=0&amp;receiveId=67' \<br /><li>&nbsp; &nbsp;&nbsp; &nbsp;&nbsp; &nbsp; --header 'token: ${{ secrets.TOKEN }}'<br /><li></ol></div><em onclick="copycode($('code_Arz'));">复制代码</em></div><br />
<br />
创建个github action 塞进去，把${{ secrets.TOKEN }}换成你的（注意要private不然被人拿走了），或者加个secrets。<br />
<br />
不知token多久过期，也不知道方法行不行，没第二个号测试，也没等token过期。<br />
不行再改改
