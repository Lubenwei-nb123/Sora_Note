# Sora技术路线详解

Sora模型不仅是一个视频生成模型，也算是一个世界模拟器。

## 模型训练流程

![训练流程](D:\Book Worm\Sora_Note\pic\训练流程.png)

Sora是一个在不同时长、分辨率和宽高比的视频及图像上训练生成的**Diffusion模型**，同时采用了**transformer架构**。

其中Diffusion模型是基于非平衡热力学概念，通过马尔可夫链构建数据样本，示意图如下：

![image-20240229225639221](D:\Book Worm\Sora_Note\pic\diffusion transformer.png)

