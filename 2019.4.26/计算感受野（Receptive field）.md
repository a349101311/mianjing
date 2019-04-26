# 计算感受野（Receptive field）

## 一、定义

The receptive field is defined as the region in the input space that a particular CNN's feature is looking at(i.e. be affected by).

在卷积神经网络中，感受野的定义是 卷积神经网络每一层输出的特征图上的像素点在原始图像上映射的区域大小。

## 二、计算感受野的一个网站

https://fomoro.com/projects/project/receptive-field-calculator

## 三、感受野计算公式

![1556283308323](C:\Users\zhangqi\AppData\Roaming\Typora\typora-user-images\1556283308323.png)

lk-1是第k-1层的感受野大小，fk是当前层的卷积核大小，si是第i层的步长。

## 四、增加感受野的大小

图像分割模型DeepLab采用了扩展卷积（Atrous Convolution，Dilated Convolution）来增加感受野大小。