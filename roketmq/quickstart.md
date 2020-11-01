相关配置
1.启动namesrv，需要配置ROCKETMQ_HOME，源代码所在路径
  ROCKETMQ_HOME=/Users/oscar/Downloads/1.0学习资料/2.后端学习/2.0 RocketMQ学习/rocketmq
  提示The Name Server boot success. serializeType=JSON 表示启动成功
2.启动broker，需配置ROCKETMQ_HOME 和 NAMESRV_ADDR
  ROCKETMQ_HOME=/Users/oscar/Downloads/1.0学习资料/2.后端学习/2.0 RocketMQ学习/rocketmq
  NAMESRV_ADDR=127.0.0.1:9876
  提示The broker[192.168.0.104, 192.168.0.104:10911] boot success. serializeType=JSON and name server is 127.0.0.1:9876 表示启动成功
  切记，and name server is 127.0.0.1:9876 表示启动成功必须要有，不然启动producer会报错，
  另外NAMESRV_ADDR=127.0.0.1:9876一定不能漏，否则会报错No route info of this topic, TopicTest
