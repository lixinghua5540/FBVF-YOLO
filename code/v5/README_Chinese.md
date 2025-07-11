# YOLOv5-FBV-Fusion

## YOLOv5
首先FBV-Fusion的创作团队非常感谢YOLOv5的创作团队，我们的FBV-Fusion在YOLOv5基础上的改进，本工程包含了YOLOv5的原始的代码。

##
YOLOv5 🚀 是世界上最受欢迎的视觉 AI，代表<a href="https://www.ultralytics.com/"> Ultralytics </a>对未来视觉 AI 方法的开源研究，结合在数千小时的研究和开发中积累的经验教训和最佳实践。

我们希望这里的资源能帮助您充分利用 YOLOv5。请浏览 YOLOv5 <a href="https://docs.ultralytics.com/yolov5/">文档</a> 了解详细信息，在 <a href="https://github.com/ultralytics/yolov5/issues/new/choose">GitHub</a> 上提交问题以获得支持，并加入我们的 <a href="https://discord.com/invite/ultralytics">Discord</a> 社区进行问题和讨论！

如需申请企业许可，请在 [Ultralytics Licensing](https://www.ultralytics.com/license) 处填写表格

# 如何使用
## 1.本地部署

### 下载本工程到本地

### 配置环境

conda create -n yolov5 python=3.8.20
conda activate yolov5
pip install -r requirements.txt

## 2.训练、测试数据配置

### 下载YOLO格式的训练数据到本地，并且新建或修改./data/数据集名称.yaml
例如：
train: /home/bxc/STOD/train/ImageName.txt (训练数据位置)
val: /home/bxc/STOD/val/ImageName.txt (验证数据位置)
test: /home/bxc/STOD/val/ImageName.txt (测试数据位置)

nc: 5 (数据类别总数)

names: ['Small Vehicle', 'Large Vehicle', 'Ship', 'Airplane', 'Oil Tank'] （数据类别名称，按顺序对应）

## 3.开始训练

### 配置数据文件

修改train.py第570行为：

parser.add_argument("--data", type=str, default=ROOT / "data/数据集名称.yaml", help="dataset.yaml path"

### 更换模型

若要更换模型为YOLOv5的原版模型，请修改train.py的第569行（我们的模型为models/yolov5-mask.yaml）

parser.add_argument("--cfg", type=str, default="models/yolov5.yaml", help="model.yaml path")
