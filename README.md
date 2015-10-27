# java-multithread-pattern

总结java中12中多线程设计模式，由于从java单线程程序开始到javaNIO，直接跳跃的去学习，就没有很好的过渡性，也就是会不懂java NIO，所以这里也算是java single thread 到java NIO之间的一座桥梁吧!


--------------------
<div id="toc">
### 目录


- [Single Threaded Execution Patern](#single-thread)
- [Immutable Pattern](#immutable-pattern)
- [Guarded Suspension Pattern](#guarded-suspension)
- [Balking Pattern](#balking-pattern)
- [Producer-Consumer Pattern](#producer-consumer)
- [Read-Write Lock Pattern](#read-write-lock)
- [Thread-Per_Message Patterm](#thread-per-message)
- [Worker Thread Pattern](#work-thread)
- [Future Pattern](#future-pattern)
- [Two-Phase Termination Pattern](#two-phase-termination)
- [Thread-Specific Storage Pattern](#thread-specific-storage)
- [Active Object Pattern](#active-object)


##关于java多线程不错的参考文献##

- [如果我是国王：关于解决 Java 编程语言线程问题的建议](https://www.ibm.com/developerworks/cn/java/j-king/)
 - [The Java™ Tutorials](https://docs.oracle.com/javase/tutorial/essential/concurrency/index.html)
 - [A Guide to Multithreaded Programming](http://www8.cs.umu.se/kurser/TDBC64/VT03/pthreads/pthread-primer.pdf)
 - 	[2001年sun开的JavaOne大会上Allen I. Holub的演讲](http://denninginstitute.com/pjd/cs571/RES/javathreads.pdf)
 - [Taming Java Threads书籍](http://read.pudn.com/downloads127/ebook/539452/Apress-Taming-Java-Threads.pdf)

- [Doug Lea's Home Page](http://g.oswego.edu/dl/):可以获取多线程的类链接库util.concurrent