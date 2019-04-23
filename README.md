# SVD+prune加速深度神经网络
 运用SVD分解与prune加速深度神经网络,对给定的深度学习神经网络在不进行参数训练的情况下，通过修改网络结构，参数优化达到减少网络运行消耗的时间，减小网络运行占用的显存同时保持与原网络相当的准确率。此次网络压缩采用的方案是对全连接层采用SVD分解，对卷积层filter采用prune法，减去每一层卷积中，权值绝对值之和最小的卷积核。<br>
 运行环境：ubuntu18.04，caffe，jupyter notebook.<br>
 首先根据prototxt文件整理出整个网络的结构，包括每一层网络的类型（conv,BN,Scale,Relu,Concat,eltwise,FF）,各个层之间的连接关系，各个层的权重系数数量；<br>
 以下是参考链接，引用时请注明出处<br>
 [SVD分解的python代码实现，非调库](https://www.cnblogs.com/endlesscoding/p/10058532.html)<br>
 [SVD全连接层分解的caffe操作](https://blog.csdn.net/zs19960124/article/details/84852538)<br>
 [张量分解实现神经网络加速有SVD，CP分解和Tucker分解（也称为高阶SVD或其他名称）](https://www.leiphone.com/news/201802/tSRogb7n8SFAQ6Yj.html)<br>
 [深度学习网络加速与压缩系列文章](https://blog.csdn.net/wspba/article/details/75671573)<br>
