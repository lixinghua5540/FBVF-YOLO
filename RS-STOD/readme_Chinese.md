# 数据集介绍：RS-STOD小目标检测数据集（用于遥感任务）
本项目中使用的数据集专为遥感图像中的小目标检测任务设计，涵盖了多种小尺度目标类型，适合用于目标检测模型的训练与评估，特别是在密集分布、低对比度和遮挡情况下的小目标识别场景。

## 📦 数据集内容
该数据集包含如下内容（按照 YOLO 标注格式组织）：

images/：图像文件，分辨率统一，采用 JPEG/PNG 格式

labels/：对应的目标检测标签（YOLO 格式）

classes.txt：类别名称列表，每行一个类别名称，对应 YOLO 中的 category_id

## 📊 数据统计
子集	图像数量	标注框数量	备注
Train	XXXX	XXXX	-
Val	XXXX	XXXX	-
Test	XXXX	XXXX	用于模型评估

注：小目标定义为 bbox 最长边小于 32 像素

## 🔗 数据下载链接
完整数据集已上传至百度网盘：

百度网盘永久链接：
📎 点击下载数据集
🔑 提取码：xxxx

## ⚠️ 请合理使用数据集，仅限科研用途，禁止商用或再分发。

## 📄 引用格式
如您在研究中使用了该数据集，请引用以下格式或本项目链接：

bibtex
@misc{your_dataset,
  title={A Remote Sensing Small Object Detection Dataset},
  author={Your Name},
  year={2025},
  url={https://github.com/yourusername/your-repo}
}
