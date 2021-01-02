# 3O机器上如何安装 Tensorflow Serving


3O机器上如何安装 Tensorflow Serving<br />
折腾了一天了 还是不行<br />
我使用 rockyzhengwu 的 nsfw<br />
运行提示如下<br />
root@sd-159807:~/nsfw# ./start_tensorflow_serving.sh<br />
./start_tensorflow_serving.sh: line 5:&nbsp;&nbsp;9834 Illegal instruction&nbsp; &nbsp;&nbsp;&nbsp;tensorflow_model_server --port=8600 --rest_api_port=8601 --model_name=${MODEL_NAME} --model_base_path=${MODEL_BASE_PATH}<br />
<br />
root@sd-159807:~/nsfw# python3 nsfw_predict.py 6rbDSaZ.jpg<br />
Illegal instruction<br />
<br />
根据以上提示 貌似使用Docker安装的 Tensorflow Serving<br />
奇怪的是 连Docker也没法安装&nbsp;&nbsp;或者安装了居然是用不了 或不会使用。<br />
<br />
<br />


帮顶，小白不会<br />
<br />
等技术大佬回答！<br />
<br />
<img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" /><img src="static/image/smiley/default/hug.gif" smilieid="13" border="0" alt="" />

不懂帮顶
