## Apache RocketMQ-remark 添加中文注释 版本4.6.1

RocketMQ源码主要分为以下几个package：
* `rocketmq-broker（broker）`：mq的核心，它能接收producer和consumer的请求，并调用store层服务对消息进行处理。HA服务的基本单元，支持同步双写，异步双写等模式。

* `rocketmq-client(client)`：mq客户端实现，目前官方仅仅开源了java版本的mq客户端，c++，go客户端有社区开源贡献。

* `rocketmq-common(common)`：一些模块间通用的功能类，比如一些配置文件、常量。

* `rocketmq-example(example)`：官方提供的例子，对典型的功能比如order message，push consumer，pull consumer的用法进行了示范。

* `rocketmq-filter(filter)`：消息过滤服务，相当于在broker和consumer中间加入了一个filter代理。

* `rocketmq-namesrv(namesrc)`：命名服务，更新和路由发现 broker服务。

* `rocketmq-remoting(remoting)`：基于netty的底层通信实现，所有服务间的交互都基于此模块。

* `rocketmq-srvutil(srvutil)`：解析命令行的工具类ServerUtil。

* `rocketmq-store(store)`：存储层实现，同时包括了索引服务，高可用HA服务实现。

* `rocketmq-tools(tools)`：mq集群管理工具，提供了消息查询等功能。

