### 关于项目

本项目代码主要来源于

https://github.com/WZMIAOMIAO/deep-learning-for-image-processing/tree/master/pytorch_classification/Test2_alexnet

在此基础上进行了书写了一些注释，本身alexnet的模型结构非常简单，所以注释不多。

```
  ├── model.py: AlexNet模型搭建
  ├── train.py: 训练脚本
  ├── predict.py: 单张图像预测脚本
  └── split_data.py：花分类数据集划分训练验证脚本
```

### 训练数据

本项目使用的是花分类数据集，首先需要下载花分类数据集，链接为

http://download.tensorflow.org/example_images/flower_photos.tgz

然后将数据集flower_photos解压放在flower_data文件夹内部，在flower_data同级目录下放置split_data.py文件，运行split_data.py划分训练验证数据集。

```
  ├── flower_data
  	  └── flower_photos
  	      ├── daisy
  	      ├── dandelion
  	      └── roses ...  
  └── split_data.py: 批量图像预测脚本
```

划分好训练数据集后，更改train.py文件的数据集路径（31行），即可训练。

CSDN上一个关于介绍花分类数据集的用法的博客

https://blog.csdn.net/qq_62932195/article/details/122094111

个人关于Alexnet的解读文章

https://zhuanlan.zhihu.com/p/460891496

