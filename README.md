# paper-list

## 2010 A Classification Scheme for Lymphocyte Segmentation in H&E Stained Histology Images
提出了一种自动检测组织病理学图像中的淋巴细胞的技术。拟议的系统将H＆E染色的数字彩色图像作为输入，以识别淋巴细胞。该过程涉及从细胞外基质中进行细胞分割，特征提取，分类和重叠分辨率。细胞外基质分割是对图像进行等效于HSV的两步过程，使用基于均值漂移的聚类进行颜色逼近，然后在HSV空间中进行阈值分割。从细胞中提取的纹理特征用于训练SVM分类器，该分类器用于对淋巴细胞和非淋巴细胞进行分类。基于轮廓的重叠分辨率技术用于解析重叠的淋巴细胞。
关键字：淋巴细胞，分类，轮廓重叠分辨率。
### Feature Extraction
The mask obtained from the previous steps represented lymphocytes as digital number 1 and other areas as digital number 0. This mask was multiplied with the histogram equalized grayscale image of the RGB image shown in figure 2(a).
Histogram equalization was performed to normalize varying illumination con- ditions. Eighteen texture features were extracted for every detected cell region [17,18,3]. These are – Autocorrelation, Contrast, Correlation, Cluster Promi- nence, Cluster Shade, Dissimilarity, Energy, Entropy, Homogeneity, Maximum probability, Variance, Sum average, Sum variance, Sum entropy, Difference vari- ance, Difference entropy, Information measure of correlation, Normalized inverse difference moment [17,18,3]. These features were derived from the gray level co- occurence matrix for four values of offset and four values of direction. Average of these eight values was used as feature value in classification.