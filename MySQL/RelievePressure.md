## 缓解读写压力

1. 主从配置
1. Redis/memcache: 适用于读取频繁，变更较小的数据
1. 负载均衡
1. 拆分数据库


LVS
  - 属于回层代理，值进行分发，效率高
  - 工作稳定，可进行高可用配置
  - 无流量，不影响主机网络


拆分数据库（分配至不同轮询中）
1. 按需建立新的数据库集群（与老集群建立主从关系)
1. 同步数据
1. 迁移数据库账号到新集群
1. 修改数据库连接