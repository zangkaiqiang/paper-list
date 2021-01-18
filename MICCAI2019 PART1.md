# MICCAI2019 PART1

## Multi-scale Cell Instance Segmentation with Keypoint Graph Based Bounding Boxes
Abstract. Most existing methods handle cell instance segmentation problems directly without relying on additional detection boxes. These methods generally fails to separate touching cells due to the lack of global understanding of the objects. In contrast, box-based instance segmenta- tion solves this problem by combining object detection with segmenta- tion. However, existing methods typically utilize anchor box-based detec- tors, which would lead to inferior instance segmentation performance due to the class imbalance issue. In this paper, we propose a new box-based cell instance segmentation method. In particular, we first detect the five pre-defined points of a cell via keypoints detection. Then we group these points according to a keypoint graph and subsequently extract the bounding box for each cell. Finally, cell segmentation is performed on fea- ture maps within the bounding boxes. We validate our method on two cell datasets with distinct object shapes, and empirically demonstrate the superiority of our method compared to other instance segmenta- tion techniques. Code is available at: https://github.com/yijingru/KG Instance Segmentation.

大多数现有方法直接处理单元实例分割问题，而无需依赖其他检测框。由于缺乏对物体的整体了解，这些方法通常无法分离触摸单元。相反，基于盒子的实例分割通过将对象检测与分割相结合来解决此问题。但是，现有方法通常使用基于锚框的检测器，由于类不平衡问题，这将导致实例分割性能下降。在本文中，我们提出了一种新的基于盒子的单元格实例分割方法。特别是，我们首先通过关键点检测来检测单元格的五个预定义点。然后，我们根据关键点图将这些点分组，然后为每个单元格提取边界框。最后，对边界框内的特征图执行细胞分割。我们在具有不同对象形状的两个单元格数据集上验证了我们的方法，并通过经验证明了该方法与其他实例分割技术相比的优越性。可以从以下网址获得代码：https://github.com/yijingru/KG实例分段。


## Improving Nuclei/Gland Instance Segmentation in Histopathology Images by Full Resolution Neural Network and Spatial Constrained Loss

Abstract. Image segmentation plays an important role in pathology image analysis as the accurate separation of nuclei or glands is crucial for cancer diagnosis and other clinical analyses. The networks and cross entropy loss in current deep learning-based segmentation methods orig- inate from image classification tasks and have drawbacks for segmen- tation. In this paper, we propose a full resolution convolutional neural network (FullNet) that maintains full resolution feature maps to improve the localization accuracy. We also propose a variance constrained cross entropy (varCE) loss that encourages the network to learn the spa- tial relationship between pixels in the same instance. Experiments on a nuclei segmentation dataset and the 2015 MICCAI Gland Segmenta- tion Challenge dataset show that the proposed FullNet with the varCE loss achieves state-of-the-art performance. The code is publicly available (https://github.com/huiqu18/FullNet- varCE).


图像分割在病理图像分析中起着重要作用，因为准确分离核或腺对于癌症诊断和其他临床分析至关重要。 当前基于深度学习的分割方法中的网络和交叉熵损失源自图像分类任务，并且存在分割缺陷。 在本文中，我们提出了一种全分辨率卷积神经网络（FullNet），该网络维护全分辨率特征图以提高定位精度。 我们还提出了方差约束交叉熵（varCE）损失，该损失鼓励网络学习同一实例中像素之间的空间关系。 在原子核分割数据集和2015 MICCAI腺体分割挑战数据集上进行的实验表明，所提出的具有varCE损失的FullNet具有最先进的性能。 该代码是公开可用的（https://github.com/huiqu18/FullNet-varCE）。


## ET-Net: A Generic Edge-aTtention Guidance Network for Medical Image Segmentation
分割是医学图像分析中的一项基本任务。但是，大多数现有方法都集中在主要区域提取上，而忽略了边缘信息，这对于获得准确的分割很有用。在本文中，我们提出了一种通用的医学分割方法，称为Edge-aTtention指导网络（ET-Net），该方法嵌入了边缘注意表示以指导分割网络。具体而言，利用边缘引导模块来学习早期编码层中的边缘关注表示，然后将其转移到使用加权聚合模块融合的多尺度解码层中。在四个分割任务上的实验结果（即视网膜图像中的视盘/杯和血管分割，以及胸部X射线和CT图像中的肺分割）表明，保留边缘注意表示有助于最终的分割精度，并且我们提出的方法优于目前的最新细分方法。我们方法的源代码可从https://github.com/ZzzJzzZ/ETNet获得。

## Deep Segmentation-Emendation Model for Gland Instance Segmentation
准确，自动化的腺体组织切片显微镜图像可以帮助病理学家诊断大肠腺癌的恶性程度。为了解决这个问题，已经提出了许多基于深度卷积神经网络（DCNN）的方法，其中大多数旨在通过改进模型结构和损失函数来产生更好的分割。但是，他们中很少有人专注于进一步推论推断的预测，从而错过了完善获得的分割结果的机会。在本文中，我们提出了用于腺体实例分割的深度分割-修正（DSE）模型。该模型由一个细分网络（Seg-Net）和一个修正网络（Eme-Net）组成。 Seg-Net专门用于生成分割结果，而Eme-Net学会预测地面实况与Seg-Net生成的分割结果之间的不一致。 Eme-Net所做的预测可以反过来用于细分结果。我们针对2015年MIC-CAI腺体分割挑战（GlaS）数据集上的五个最新深度学习模型以及针对结直肠腺癌（CRAG）数据集上的两个深度学习模型，评估了我们的DSE模型。我们的结果表明，使用Eme-Net可以显着提高分割精度，并且在两个数据集的腺体实例分割中，所提出的DSE模型都能够大大胜过所有其他模型。