# 中文文本分类
主要描述的是中文分类中的一些疑问，理解问题最好的方法就是实践
## 比较好的网站推荐
1，[详解卷积神经网络CNN](—详解卷积神经网络CNN)  
2,
## 问题集合
1，TextCNN如何确定min-batch-size的？  
答：有文章支出不小于训练集\1000<sup>[1]</sup>

2，TextCNN如何处理连续的两个卷积层的？    
答：第一次使用的卷积核大小为(filter-size, embeddimg)，其后使用的卷积核尺寸为(filter-size, 1)    

3，如果在提取预训练模型中的词向量时没有，会发生什么？  
答：对于该词进行随机初试化<sup>[2]</sup>

4，如何解决神经网络训练时loss不下降的问题？  
答：正则过度、初始化方案有问题<sup>[3]</sup>
## 参考文献
1，[关于cnn 文本分类参数调节总结](https://blog.csdn.net/qq_32023541/article/details/80984624)  
2，[TextCNN:CNN for Sentence Classification](https://zhuanlan.zhihu.com/p/78355881)  
3，[如何解决神经网络训练时loss不下降的问题](https://blog.ailemon.me/2019/02/26/solution-to-loss-doesnt-drop-in-nn-train/)