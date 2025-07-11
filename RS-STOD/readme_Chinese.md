# 数据集介绍：RS-STOD小目标检测数据集（用于遥感任务）
本项目中使用的数据集专为遥感图像中的小目标检测任务设计，涵盖了多种小尺度目标类型，适合用于目标检测模型的训练与评估，特别是在密集分布、低对比度和遮挡情况下的小目标识别场景。
注：小目标定义为 bbox 最长边小于 32 像素， 超微小目标定义为 bbox 最长边小于 16 像素

## 📦 数据集内容
该数据集包含两种标注格式：YOLO格式与COCO格式，分别放置在对应名称的文件夹中。

其中coco格式进行了train与val的划分，YOLO格式未进行划分。

classes.txt：类别名称列表，每行一个类别名称，对应 COCO 中的 category_id

数据集的详细信息请参阅我们的论文：A front-back view fusion strategy and a novel dataset for super tiny object detection in remote sensing imagery

## 🔗 数据下载链接
完整数据集已上传至百度网盘：

百度网盘永久链接：

点击下载数据集

📎 链接：https://pan.baidu.com/s/1jO7W3mQ07Ec0xHcnTC0ANg?pwd=2u3z 

🔑提取码：2u3z 

## ⚠️⚠️⚠️ 请合理使用数据集，仅限科研用途，禁止商用或再分发！ ⚠️⚠️⚠️

## 📄 引用格式
如您在研究中使用了该数据集，请引用以下格式：

bibtex
@article{BAI2025114051,

  title = {A front-back view fusion strategy and a novel dataset for super tiny object detection in remote sensing imagery},
  journal = {Knowledge-Based Systems},
  volume = {326},
  pages = {114051},
  year = {2025},
  doi = {https://doi.org/10.1016/j.knosys.2025.114051},
  author = {Xuechen Bai and Xinghua Li and Jianhao Miao and Huanfeng Shen},
}
