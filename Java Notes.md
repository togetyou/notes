### 集合框架

### 并发编程
    List
    CopyOnWriteList
    Queue (add offer poll peek)
        add 和 offer的区别
        CocurrentLinkedQueue
        BlokingQueue(put ,take)  put方法满了会阻塞
            LinkedBlockingQueue 无界队列
            ArrrayBlockingQueue 有界队列
        DelayQueue  无界队列  （应用场景 delay获取）
        TransferQueue  提一个transfer方法,transfer方法生产者往队列里面放对象的时候先看下有有没有消费者线程等待先给消费者线程否则等待
        SynchronusQueue 容量为0的TransferQueue队列,每个对象必须直接被消费者线程消费

#### 线程池
    Callable 有返回值，并且抛出异常
    Runnable 没有返回值 且不能抛出异常
    Excutor
    ExcutorService
    6种线程池
    ThreadPoolExcutor
##### 线程池问题
    线程池各个参数的意义？
    如何自己实现一个线程池？
    使用预定的6种线程池有什么问题？

### 设计模式
#### 观察者模式
    三个要素：观察者 事件源 事件  
    特别明显的应用在 UI事件编程，响应式编程里面
    设计一个观察者模式：垂钓？

### 注解
### Java8 Lambada 表达式

### 问题
    Thread.sleep TimeUnits.Sesconds.sleep 区别？
    各种线程池相关的队列 ？
    各种队列的使用
    parallelStream?
    cas是什么?
