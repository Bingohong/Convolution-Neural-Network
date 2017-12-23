# CNN visualization
Based on the paper [2013-Visualizing and Understanding Convolutional Networks](https://www.cs.nyu.edu/~fergus/papers/zeilerECCV2014.pdf) by Matthew D. Zeiler and Rob Fergus.,
the code is referenced from [tf_cnnvis](https://github.com/InFoCusp/tf_cnnvis).
It use the [TensorFlow](https://tensorflow.google.cn/) library at the backend and the generated images are displayed in [TensorBoard](https://tensorflow.google.cn/get_started/summaries_and_tensorboard).
There are implemented 2 CNN visualization techniques:
1. The goal here is to reconstruct the input image from the information contained in any given layers of the convolutional neural network.
2. CNN visualization based on [Deep dream](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/tutorials/deepdream/deepdream.ipynb) by Google.
Here's the relevant [blog post](https://research.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html) explaining the technique.
In essence, it attempts to construct an input image that maximizes the activation for a given output.

# CNN 卷积可视化
可视化方法基于论文[2013-Visualizing and Understanding Convolutional Networks](https://www.cs.nyu.edu/~fergus/papers/zeilerECCV2014.pdf)，
代码参考于[tf_cnnvis](https://github.com/InFoCusp/tf_cnnvis)。这里使用[TensorFlow](https://tensorflow.google.cn/)作为后端计算引擎，并且将生成的图片展示在[TensorBoard](https://tensorflow.google.cn/get_started/summaries_and_tensorboard).
这里主要完成2种可视化技术：
1. 重构给定卷积层的输入图像，反卷积方法
2. 根据给定的输出，构建可使激活函数最大(maximizes the activation)的输入图像。Google的[Deep dream](https://github.com/tensorflow/tensorflow/blob/master/tensorflow/examples/tutorials/deepdream/deepdream.ipynb).
相关[博客](https://research.googleblog.com/2015/06/inceptionism-going-deeper-into-neural.html)解释了这个技术。
