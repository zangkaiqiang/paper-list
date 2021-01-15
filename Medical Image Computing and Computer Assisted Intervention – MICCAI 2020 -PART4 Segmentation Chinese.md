# Medical Image Computing and Computer Assisted Intervention – MICCAI 2020 -PART4 Segmentation



## Deep Volumetric Universal Lesion Detection Using Light-Weight Pseudo 3D Convolution and Surface Point Regression



Abstract 

从患者的CT扫描中准确，全面地识别，测量和报告病变对医生而言是重要且耗时的过程。计算机辅助病变/重大发现检测技术是医学成像的核心，由于病变外观，位置和大小分布在3D成像中存在极大的变异性，因此仍然非常具有挑战性。在这项工作中，我们提出了一种新颖的深层无锚固式一级体积病灶检测器（VLD）框架，该框架结合了（1）伪3D卷积运算符，可以从现成的框架中循环利用架构配置和预先训练的权重2D网络，尤其是具有处理数据差异的能力的网络，以及（2）一种新的表面点回归方法，可通过在病变表面上精确定位3D病变空间的代表性关键点来有效地回归3D病变空间范围。首先在公共大型NIH DeepLesion数据集上进行实验验证，我们提出的方法可提供最新的定量性能。我们还在内部数据集上测试VLD以检测肝肿瘤。 VLD在CT成像的大型和小型肿瘤数据集中都能很好地概括。



## DeScarGAN: Disease-Specific Anomaly Detection with Weak Supervision

医学图像中的异常检测和定位是一项艰巨的任务，尤其是当异常表现出现有结构的变化（例如，脑萎缩或由于胸腔积液引起的胸膜腔变化）时。在这项工作中，我们提出了一种弱监督和细节保留的方法，该方法能够检测现有解剖结构的结构变化。与标准异常检测方法相反，我们的方法从两组中提取有关疾病特征的信息：一组受同一疾病影响的患者和一个健康对照组。结合身份保存机制，这使我们的方法能够提取高度疾病特异性的特征，以更详细地检测结构变化。我们设计了一个特定的综合数据集，以评估和比较我们的方法与最新的异常检测方法。最后，我们在胸部X射线图像上显示了我们方法的性能。我们的方法DeScarGAN在合成数据集上以及通过对胸部X射线图像数据集的目测检查均胜过其他异常检测方法。



## KISEG: A Three-Stage Segmentation Framework for Multi-level Acceleration of Chest CT Scans from COVID-19 Patients

在持续的COVID-19暴发期间，通过计算机断层扫描（CT）对COVID-19肺炎进行准确诊断至关重要。尽管胸部病变分割在计算机辅助诊断（CAD）中起着关键作用，但是由于缺乏公开可用的带有手动注释的CT数据集而影响了准确性。另外，对于临床部署而言，如何在语义分割模型的准确性和效率之间取得平衡仍然是一个挑战。为了解决这些问题，我们构建了第一个带有像素病灶注释的COVID-19肺炎的CT数据集。我们提出了一个称为KISEG（分割的关键和中间帧）的三阶段框架，以通过多级加速来增强串行CT图像分割的性能。我们首先采取一项策略，将串行CT的帧分为两组，即关键帧和中间帧。然后，KISEG使用主要模型（准确但繁琐）进行关键帧分割。第三，采用辅助模型进行中间帧分割，并融合融合模块中的关键帧信息。此外，我们提出了一个高斯核dropout来进行数据增强。在我们的数据集上进行的实验表明，我们提出的KISEG模型对比state of the art方法可以达到相当的精度，并且需要更少的算力，速度从2.88x提高到9.16x。该数据集已公开发布，可用于AI社区的COVID-19的进一步研究，已在http://ncov-ai.big.ac.cn/download上发布。



## **CircleNet: Anchor-Free Glomerulus Detection with Circle Representation**

物体检测神经网络在计算机视觉方面功能强大，但对生物医学物体检测并没有进行必要的优化。 在这项工作中，我们提出了CircleNet，这是一种简单的无锚（anchor-free）检测方法，可以用圆形表示来检测球形肾小球。 与传统的基于边界框的检测方法不同，边界圆（1）降低了检测表示的自由度，（2）是旋转不变的，（3）并针对球形物体进行了优化。 实现这种表示的关键创新是带有圆检测头的无锚框架。 我们在检测肾小球的背景下评估CircleNet。 CircleNet将肾小球检测的平均精度从0.598提高到0.647。 与边界框表示相比，CircleNet的另一个主要优点是其旋转一致性更好。



## Weakly Supervised One-Stage Vision and Language Disease Detection Using Large Scale Pneumonia and Pneumothorax Studies

尽管数据集很大，但是缺少详细的标签，所以要在医学图像中检测临床相关对象仍然是一个挑战。为了解决标签问题，我们将场景级别的标签与包含自然语言信息的检测架构结合使用。我们在公开可用的MIMIC-CXR数据集上特别是肺炎和气胸的放射线学上，提出了一组具有挑战性的放射线学家配对的边界框和自然语言注释。连同数据集一起，我们提出了一种联合视觉语言，由弱监督的变压器层选择的 one-stage双头检测架构（LITERATI），以及与类激活映射（CAM），梯度CAM和NIH上的相关实现的强基线比较ChestXray-14和MIMIC-CXR数据集。 LITERATI方法借鉴了视觉语言体系结构的先进性，展示了联合图像和参考表达（使用自然语言在图像中定位的对象）输入以进行检测，并以纯弱监督的方式进行缩放。架构上的修改解决了三个障碍：以弱监督的方式实施有监督的视觉和语言检测方法，结合临床指称表达自然语言信息以及生成具有地图概率的高保真检测。尽管如此，放射线医师注释具有挑战性的临床性质，包括细微的参考，多实例规范以及相对冗长的基础医学报告，确保了大规模的视觉语言检测任务仍在刺激中，以备将来研究之用。

??



## Diagnostic Assessment of Deep Learning Algorithms for Detection and Segmentation of Lesion in Mammographic Images

深度学习算法在乳腺X射线图像病变检测和分割中的诊断评估



计算机辅助检测或诊断支持方法旨在通过帮助放射科医生评估数字化X线摄影（DM）检查来改善乳腺癌筛查程序。该系统涉及深度学习在早期阶段对软组织病变的自动检测和分割的用途。本文提出了一种新颖的深度学习方法，该方法基于two stage目标检测器，该目标检测器将增强的Faster R-CNN与Libra R-CNN结构结合在一起用于目标检测分割。分割网络放置在先前结构的顶部，以提供各种特征（即边缘，形状）的精确提取和定位。分割头基于递归残差卷积神经网络(Recurrent Residual Convolutional Neural Network)，可以针对特定实例属性进行附加特征分类。从一家供应商Hologic收集了一个数字乳房X线照片的数据库，其中有1200张图像包含了肿块。我们的自动检测系统的性能通过模型的灵敏度进行了评估，模型的灵敏度达到了微平均召回率：0.892，微平均精度：0.734，微平均F1得分：0.805。宏观平均召回率：0.896，宏观平均准确度：0.819，宏观平均F1得分：0.843。对同一测试集的分段性能评估为平均IOU为0.859。



## Efficient and Phase-Aware Video Super-Resolution for Cardiac MRI

高效的相位感知视频
心脏MRI的超分辨率

心脏磁共振成像（CMR）被广泛使用，因为它可以以无创，无痛的方式说明心脏的结构和功能。但是，由于硬件的限制，获取高质量的扫描既费时又费钱。为此，我们提出了一种新颖的端到端可训练网络，以解决CMR视频超分辨率问题，而无需硬件升级和扫描协议修改。我们将心脏知识整合到我们的模型中，以帮助利用时间信息。具体来说，我们将心脏知识公式化为周期性函数，以适应CMR的周期性特征。此外，提出的残差学习方案的残差有助于网络以渐进的改进方式学习LR-HR映射。通过根据任务的难度调整细化迭代，该机制使网络具有自适应能力。与大量最新方法相比，大规模数据集上的大量实验结果证明了该方法的优越性。



## ImageCHD: A 3D Computed Tomography Image Dataset for Classification of Congenital Heart Disease

ImageCHD：用于先天性心脏病分类的3D计算机断层扫描图像数据集

先天性心脏病（CHD）是最常见的出生缺陷类型，在美国，每110胎中就有1例发生。冠心病通常会伴随心脏结构和大动脉连接的严重变化，可分为多种类型。因此，需要高度专业化的领域知识和费时的人工过程来分析相关的医学图像。另一方面，由于冠心病的复杂性和缺乏数据集，关于冠心病的自动诊断（分类）的研究很少。在本文中，我们介绍了ImageCHD，这是第一个用于CHD分类的医学图像数据集。 ImageCHD包含110种3D计算机断层扫描（CT）图像，涵盖了大多数类型的CHD，与现有医学影像数据集相比，其尺寸还不错。冠心病的分类要求鉴定大的结构变化而没有任何局部组织变化，并且数据有限。这是一类较大的问题的例子，对于当前基于机器学习的视觉方法来说，这些问题很难解决。为了证明这一点，我们进一步介绍了基于最新的CHD分割方法的CHD自动分类的基线框架。实验结果表明，在选择性预测方案下，基线框架只能实现82.0％的分类精度，覆盖率达到88.4％，为进一步改进留有很大空间。我们希望ImageCHD能够刺激进一步的研究，并导致创新和通用的解决方案，这些解决方案将在多个领域产生影响。我们的数据集已公开发布[1]。



## Deep Generative Model-Based Quality Control for Cardiac MRI Segmentation

基于深度生成模型的心脏MRI分割质量控制

近年来，卷积神经网络已在各种医学图像分割任务中表现出令人鼓舞的性能。但是，当将训练有素的细分模型部署到现实的临床世界中时，该模型可能无法达到最佳效果。一个主要的挑战是由于图像质量下降或域移位问题而产生的潜在劣质分割。迫切需要开发一种自动化的质量控制方法，该方法可以检测不良的细分并将其反馈给临床医生。在这里，我们提出了一种新颖的基于深度生成模型的心脏MRI分割质量控制框架。首先，它使用生成模型学习多种高质量的图像分割对。然后通过评估从其投影到高质量歧管上的差异来评估给定测试细分的质量。特别是，通过在潜在空间中进行迭代搜索来精炼投影。所提出的方法在两个公开可用的心脏MRI数据集上实现了很高的预测精度。而且，与传统的基于回归的方法相比，它具有更好的泛化能力。我们的方法为心脏MRI分割提供了实时且与模型无关的质量控制，它有可能集成到临床图像分析工作流程中。



## DeU-Net: Deformable U-Net for 3D Cardiac MRI Video Segmentation



## Learning Directional Feature Maps for Cardiac MRI Segmentation



## Joint Left Atrial Segmentation and Scar Quantification Based on a DNN with Spatial Encoding and Shape Attention





## XCAT-GAN for Synthesizing 3D Consistent Labeled Cardiac MR Images on Anatomically Variable XCAT Phantoms



