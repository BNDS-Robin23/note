# 均摊分析
+ 均摊分析，用于分析平均花费，经常被应用于数据结构的评估分析。

## 定义
+ Operation has amprtized cost $\hat{c_i}$  
**TODO**

## 用循环数组实现队列的均摊分析
+ 未达到数组容量上限时，使用循环数组时插入删除都是O(1)时间操作
+ 但是当数组达到容量上限时，扩容的时间开销为O(n)
+ 假设定义插入操作的均摊开销为2，删除操作的均摊开销为1，下面通过证明实际总开销小于均摊开销之和证明这样的开销分配方案是不是合理的
  + **TODO：补图**
  + 发现存在某个时刻不满足上述性质，因此均摊开销为2是不合理的
+ 