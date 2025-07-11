# FBVF-YOLO
Official repository for the paper ‘A front-back view fusion strategy for enhancing YOLO and new dataset for super tiny object detection in remote sensing imagery’, containing the STOD dataset, FBVF training, and validation code.

## Abstract
Super tiny objects (STOs) are frequently submerged in complex backgrounds of remote sensing and natural images, which brings major challenges for existing learning-based object detection methods. Currently, You Only Look Once (YOLO) is one of the most widely used mainstream methods in the field of object detection. However, its performance on STOs detection is still not satisfactory. The biggest challenge lies in the network’s difficulty in effectively extracting the scarce geometric and spectral information of STOs. Towards this end, a front-back view fusion (FBV-Fusion) strategy compatible with the famous YOLO framework is proposed. Firstly, to prevent background information from overwhelming STOs features, a target mask is generated through the YOLO backbone, dividing the feature layer into target and background regions. Then, to enhance the utilization of feature extraction in the target area and background information, the skip convolution replaces all normal convolution in YOLO neck, focusing on the features of the target region. The feature layer size is increased to mitigate the information loss of STOs at the source. Moreover, to address the scarcity of datasets and the imbalance of samples for remote sensing STOs detection, a novel dataset called super tiny object detection for remote sensing (RS-STOD) dataset was constructed. To evaluate its generalization capability and the effectiveness of FBV-Fusion, the experiments were conducted on RS-STOD, AI-TOD and TinyPerson. Meanwhile, the FBV-Fusion strategy was validated across YOLOv5, v7, v9, v10 and v11. The results demonstrate that FBV-Fusion outperforms other state-of-the-art (SOTA) methods.


## 📄 Citation Format 
If you have used our method or dataset in your research, please cite it in the following format:

<pre> bibtex 
  @article{BAI2025114051, 
  title = {A front-back view fusion strategy and a novel dataset for super tiny object detection in remote sensing imagery}, 
  author = {Xuechen Bai and Xinghua Li and Jianhao Miao and Huanfeng Shen}, 
  journal = {Knowledge-Based Systems},
  volume = {326}, 
  pages = {114051}, 
  year = {2025}, 
  doi = {https://doi.org/10.1016/j.knosys.2025.114051}, 
  }  </pre>
