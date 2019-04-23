# SVD+prune加速深度神经网络
 >运用SVD分解与prune加速深度神经网络,对给定的深度学习神经网络达到减少网络运行所消耗的时间，占用的显存同时保持与原网络相当的准确率。此次竞赛采用的是对全连接层采用SVD分解，对卷积层filter采用prune法，减去每一层卷积中，权值绝对值之和最小的卷积核。以下是参考链接，引用时请注明出处<br>
 [SVD分解的python代码实现，非调库](https://www.cnblogs.com/endlesscoding/p/10058532.html)<br>
 [SVD全连接层分解的caffe操作](https://blog.csdn.net/zs19960124/article/details/84852538)<br>
 [张量分解实现神经网络加速有SVD，CP分解和Tucker分解（也称为高阶SVD或其他名称）](https://www.leiphone.com/news/201802/tSRogb7n8SFAQ6Yj.html)<br>
