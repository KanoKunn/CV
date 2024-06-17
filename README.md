# CV课程作业

## 复现论文基本信息  

学生：魏东健

复现论文：EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything

论文来源：CVPR accepted paper 2024 

原文github链接：[yformer/EfficientSAM: EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything (github.com)](https://github.com/yformer/EfficientSAM?tab=readme-ov-file)

## 摘要

任意分段模型(SAM)已经成为许多视觉应用的强大工具。 驱动零射击传输和高通用性令人印象深刻的性能的关键组 件是在广泛的高质量SA-1B数据集上训练的超大Transforme r模型。虽然SAM模型是有益的，但其巨大的计算成本限制了其 在实际应用中的广泛应用。为了解决这一限制，我们提出了 efficientsam，这是一种轻量级的SAM模型，它表现出良好的性能， 同时大大降低了复杂性。我们的想法是基于利用蒙面图像预 训练，即SAMI，它学习从SAM图像编码器中重建特征，以实现有 效的视觉表征学习。此外，我们采用sami预训练的轻量级图像 编码器和掩码解码器来构建Effi-cientSAMs，并在SA-1B上对 模型进行微调，以实现分段任何任务。我们对多个视觉任务进 行了评估，包括图像分类、目标检测、实例分割和语义目标检测， 并发现我们提出的预训练方法SAMI始终优于其他掩模图像 预训练方法。在分割任何任务(如零采样实例分割)上，与其他 快速SAM模型相比，我们的efficientsam与sami预训练的轻量级 图像编码器表现良好，具有显着增益(例如，COCO/LVIS上的AP 为4)。

## 论文创新点

1.提出了一个利用SAM的蒙面图像预训练框架， 称为SAMI，它训练模型来重建SAM ViT-H图像编码 器的特征。我们表明，这可以大大提高图像掩码预 训练方法的性能。

2.证明了sami预训练的主干可以很好地推广到许 多任务，包括图像分类、目标检测和语义分割。提供高效的轻型SAM模型，具有最先进的质量效率权衡。

## 论文复现环境

windows 10 专业版

cpu: AMD Ryzen 7 4800H with Radeon Graphics

gpu: NVIDIA GeForce RTX 2060

详细项目环境请查看我在虚拟环境导出的[environment.yaml](https://github.com/KanoKunn/CV/blob/main/environment.yaml)

如果您需要使用我的项目环境，请按照以下代码导入：

conda env create -f environment.yaml

## 论文复现演示视频


https://github.com/KanoKunn/CV/assets/146503264/337f51cc-2b44-4628-be51-c607c6040e3d


