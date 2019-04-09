# distributed-computing-pattern
- Coordinator
  - 功能
    - 将大任务分解成小任务
    - 将小任务 分配或重新分配 给存活的 worker
    - 中间数据,垃圾数据 清理
    - 健康检查
      - 运行超时
      - 清理超时
    - 分布式 latch,管理分布式任务状态
- Worker
  - 功能
    - 获取属于自己的任务
    - 运行任务
    - 更新任务的 alivetime
- DB
  - 由 DB保证数据一致性
![img](https://raw.githubusercontent.com/leoChaoGlut/distributed-computing-pattern/master/distributed-computing-pattern.png)
