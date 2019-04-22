# CQUOJQiQu
cquoj的气球程序

准备工作
====
安装Erlang
下载链接：http://www.erlang.org/downloads
安装RabbitMQ
下载链接：https://www.rabbitmq.com/download.html
安装方法：https://baijiahao.baidu.com/s?id=1608425504960724381&wfr=spider&for=pc

python3
====
pip install pika
pip install selenium
pip install beautifulsoup4

文件介绍
====
# ac_que.json
##已发气球消息列表，开始前设置为[]
# receive.py
##获取消息，处理消息，动态获取榜单
driver.get(http://acm.cqu.edu.cn/contest_show.php?cid=比赛id#standing)
mydriver.get('file:///当前路径/0.html')
# ac_stat.py
##发送消息
0   刷新
xx:xx:xx(xx) 删除ac时间戳
# send.py
##死循环每隔20秒发送0消息刷新
##容易造成rabbitmq出现问题，所以间隔时间较长，不保证安全

# .vscode
##vscode python配置文件