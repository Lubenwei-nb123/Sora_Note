# Sora技术路线详解

Sora模型不仅是一个视频生成模型，也算是一个世界模拟器。

## 模型训练流程

![训练流程](pic\训练流程.png)

Sora是一个在不同时长、分辨率和宽高比的视频及图像上训练生成的**Diffusion模型**，同时采用了**transformer架构**。

其中Diffusion模型是基于非平衡热力学概念，通过马尔可夫链构建数据样本，示意图如下：

![image-20240229225639221](pic\diffusion transformer.png)

![image-20240301000354840](pic\DiT.png)

## 含时空编码的样本取样

![image-20240229234935997](D:\Book Worm\Sora_Note\pic\时空编码.png)

Sora内部通过图上的切块法，使得采样能包含时间和空间信息。

![image-20240229235718601](pic\Sora支持不同格式输入.png)

同时使用了NaVit技术，可以降低计算量并支持动态输入。

（看的不是很懂，后面还会更新）
