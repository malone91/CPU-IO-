# CPU-IO-
IO读写与CPU之间的关系  答案来源：百度知道。

当程序读写磁盘时，CPU就空闲下来。程序读写磁盘CPU不参与么？还有就是CPU就是负责程序指令的执行吗？

答：读写磁盘CPU只负责下达命令，当读写完一个磁盘后，CPU会得到一个反馈，从这个反馈中，CPU可以知道
读写任务是否完成。在等待反馈的时间里，CPU可以去做其他的事，或者处于空闲状态。
这是一个并行机制，读写磁盘是通过内存调度（内存控制）来完成的。CPU并不参与磁盘读写。
