# MyDocker Docker功能学习与实现 

##### Introduction 简介
基于Go语言，根据《自己动手写Docker》这本书进行Docker的实现。

##### Environment 实现环境
1. 编译器 complier：Go 10.4
2. 操作系统 Operating system: Ubuntus

##### Docker base
1. Namespace.go 
  Docker的Namespace主要用于进程视图的隔离。Namespace.go文件中实现了不同命名空间下的隔离，包括UTS,UID,PID,IPC,MOUNT,NETWORK。
2. Cgroup.go 
  Docker的Cgroup主要用于资源的限制和监控，主要包括内存资源，CPU资源等。Cgroup.go中实现了针对内存的限制。
  
 ##### GO_STUDY
 1. 学习Go语言的过程，具体参考[Go by Example 中文](http://books.studygolang.com/gobyexample/atomic-counters/)
 
##### MyDocker-1
1. 实现RUN命令版本的容器

##### Additional knowledge
1. Linux系统下的/proc文件夹记录着内核的运行时状态，实际上是一个虚拟的文件系统。/proc目录给用户提供了访问内核信息的接口。
