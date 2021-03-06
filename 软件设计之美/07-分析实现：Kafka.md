[toc]

## 07 | Kafka：如何分析一个软件的实现？

### 消息队列的模型与接口

### 关键技术

### 小结

1.  设计的第三部分：**看实现**。
    
    -   理解一个实现，是以对模型和接口的理解为前提的。
    
2.  了解系统的实现：

    -   **软件结构**
    -   **关键技术**

3.  Kafka 为例

    1.  核心模型：**消息队列**

    2.  接口：**生产、消费**

    3.  软件结构：

        -   含义：**分层**
        -   工具：结构图
        -   需要了解的：
            -   设计的**结果**
            -   设计的**动因**
        -   Kafka 架构图
            -   ![img](imgs/ee05f6c6446600da97d824591e5a4d79.jpg)

    4.  关键技术：

        -   含义：就是能够让这个软件的“实现”**与众不同**的地方。

        -   特性（思路上的突破）：**软硬结合**

            >   软件：充分利用消息队列本身的特性：**有序**。
            >
            >   硬件：Kafka 的不同之处在于，它利用了**磁盘顺序读写**的特性。顺序写的话，会大幅度减少磁头的运动，效率自然就得到大幅度的提高。
    
4.  一句话总结：**理解实现，带着自己的问题，了解软件的结构和关键的技术。**

5.  ![img](https://static001.geekbang.org/resource/image/29/ef/29c6a18e1e1313ff0e6c7aad3642f3ef.jpg)