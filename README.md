# pendingpool
TCP连接池,pendingpool维护了两个socket队列：监听队列和就绪队列。
监听队列中维护已建立好长连接(三次握手完毕)为ready状态的socket；就绪队列维护可读的busy状态的socket队列，工作原理如下：
![原理图](https://github.com/whutbd/pendingpool/blob/master/images/1.jpg)
