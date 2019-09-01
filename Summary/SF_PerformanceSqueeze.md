## PHP进阶之路

### 性能压榨  [link](https://segmentfault.com/a/1190000010455076)

#### 前端优化
1. 减少http请求
    - 减少图片、css、script 数量
    - 合并css、js、小图片，通过组件化开发，最后打包输出
    - icon、UI 做成字体，矢量高清
1. 充分利用浏览器缓存
    - expires
    - cache-control
    - last-modified
    - etag(更新版本号)
1. 分布式存储前端资源
1. 多域名访问资源
    - 多域名存储资源（浏览器对单域名并行请求书限制）
    - 同一域名易产生多数无用 cookie
1. 资源数据压缩
    - 前端代码压缩
    - 服务器 gzip
    - 图片压缩
1. 优化首屏展示速度
    - 延时、按需、异步加载
1. 标准头信息
    - 严格控制 control-type，不让浏览器自己去猜


#### Nginx优化
1. 配置优化
1. tcp/ip 优化
1. 系统配置的优化


#### PHP优化
1. php7
1. opcode
1. hugepage
1. 代码伪编译
1. 模板编译
1. xprof

#### 业务优化
1. 非侵入式开发
1. 静态化（微博）
1. 业务解耦
1. 异步思想
1. 分布式、SOA

#### MySQL优化

#### 缓存优化
1. 多级缓存
    - 请求内缓存
    - 本地缓存
    - 分布式缓存
1. 避免缓存的滥用
    - 提高缓存命中率，降低更新率
    - 抽离出变动率较大的数据
1. redis优化
    - strint 计数器
    - set 黑名单
    - zset 分页列表、排行榜
    - hashes 对象存储