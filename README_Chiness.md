# A Front-back View Fusion Strategy and A Novel Dataset for Super Tiny Object Detection in Remote Sensing Imagery

## 摘要
### 中文版
超小型物体（STO）的特征常常会淹没在遥感、自然图像的复杂背景中，这给现有的基于学习的物体检测方法带来了巨大挑战。
目前，YOLO框架是物体检测领域应用最广泛的主流框架之一，然而，它在 STOs 检测方面的表现仍有很大的提升空间。
其中，最大的挑战在于现有网络难以有效提取STO稀缺的几何、纹理和光谱信息。为此，我们提出了一种与YOLO框架兼容的前后视图融合（FBV-Fusion）策略。
首先，为防止背景信息淹没STOs特征，我们通过YOLO骨干网络生成目标掩膜分支，将特征层划分为目标和背景区域。
然后，为了提高目标区域特征提取和背景信息的利用率，Skip-Conv取代了YOLO颈部的所有普通卷积，重点关注目标区域的特征。并且我们增加了网络中特征层的大小，以减少源头信息损失。
为了评估其泛化能力和FBV-Fusion的有效性，在RS-STOD、AI-TOD和TinyPerson上进行了实验。结果表明，FBV-Fusion优于其他SOTA方法。同时，FBV-Fusion 策略在 YOLOv5、v7、v9、v10 和 v11 中进行了验证，结果表明 FBV-Fusion 优于其他最先进的（SOTA）方法。

此外，针对遥感 STOs 检测数据集的稀缺性和样本的不平衡性，我们构建了一个名为RS-STOD的新型数据集。

### 英文版：
我们强烈建议您阅读英文摘要，以理解本研究的原始本意

Super tiny objects (STOs) are frequently submerged in complex backgrounds of remote sensing and natural images, which brings major challenges for existing learning-based object detection methods. Currently, You Only Look Once (YOLO) is one of the most widely used mainstream methods in the field of object detection. 
However, its performance on STOs detection is still not satisfactory. The biggest challenge lies in the network’s difficulty in effectively extracting the scarce geometric and spectral information of STOs. Towards this end, a front-back view fusion (FBV-Fusion) strategy compatible with the famous YOLO framework is proposed. Firstly, to prevent background information from overwhelming STOs features, a target mask is generated through the YOLO backbone, dividing the feature layer into target and background regions. 
Then, to enhance the utilization of feature extraction in the target area and background information, the skip convolution replaces all normal convolution in YOLO neck, focusing on the features of the target region. The feature layer size is increased to mitigate the information loss of STOs at the source. Moreover, to address the scarcity of datasets and the imbalance of samples for remote sensing STOs detection, a novel dataset called super tiny object detection for remote sensing (RS-STOD) dataset was constructed. To evaluate its generalization capability and the effectiveness of FBV-Fusion, the experiments were conducted on RS-STOD, AI-TOD and TinyPerson. Meanwhile, the FBV-Fusion strategy was validated across YOLOv5, v7, v9, v10 and v11. The results demonstrate that FBV-Fusion outperforms other state-of-the-art (SOTA) methods.



