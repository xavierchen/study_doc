## Redis持久化 ##

### RDB ###

- 指定规则
- 定时
- 内存到硬盘

- 配置规则(时间窗口、改动键个数)
- SLAVE(同步)、BGSLAVE(异步)
- FLUSHALL(定义自动快照条件)
- REPLICATION

- fork父进程生成副本子进程
- 子进程写内存
- 临时文件替换旧文件

### AOF ###

- 记录每次执行命令
- 损耗redis性能
- 自动重写
- 同步硬盘数据

### 使用方式 ###

- 各自独立使用
- 结合使用

