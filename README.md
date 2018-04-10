**基于Linux系统的MQTT服务器**

服务器基于MQTT 3.11版本，同时兼容3.1版本。目前服务器具有以下基本功能：

- 实现基本的连接、断开、心跳、订阅、发布（QoS0、QoS1、QoS2）；
- 基于UTHASH的订阅树维护；

后续将实现以下功能：

- 增加libwebsockets实现websocket通信；
- 对`retain`标识进行处理；
- 内存管理优化，实现常用结构体缓存；
- 日志输出规范化，建议运行时关闭`DEBUG`宏；
