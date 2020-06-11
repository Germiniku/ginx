# ginx
##　学习并发TCP服务器框架TCP框架Zinx
## 功能
- 实现全局配置
- 消息封装
- 多路由模式
- 读写分离模型
- 消息队列及多任务
- 连接管理
- 连接属性设置（上下文）

## 使用案例
1. 服务端Demo在ginx下的server 
2. 客户端Demo在ginx下的client
3. 配置文件下conf/zinx.json
- 目前可配置项(使用json配置文件)
```cassandraql
TcpServer       // 当前Zinx的全局server对象
Host            // 当前服务器主机IP
Port            //当前服务器主机监听端口号
Name            // 当前服务器名称
Version         // 当前Zinx版本号
WorkerPoolSize // 工作goroutine的数量
MaxPacketSize  // 数据包的最大值
MaxConn        // 当前服务器主机允许的最大连接个数
MaxMsgChanLen  // 最大的消息通道长度
```


## 待填充功能
1. 添加日志库以及记录日志
2. N+功能待实现