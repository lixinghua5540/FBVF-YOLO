# YOLOv5-FBV-Fusion

## YOLOv5
First of all, the FBV-Fusion creation team is very grateful to the creation team of YOLOv5. Our FBV-Fusion is an improvement on YOLOv5, and this project contains all of the original code of YOLOv5.

##

YOLOv5 🚀 is the world's most loved vision AI, representing <a href="https://www.ultralytics.com/">Ultralytics</a> open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.

We hope that the resources here will help you get the most out of YOLOv5. Please browse the YOLOv5 <a href="https://docs.ultralytics.com/yolov5/">Docs</a> for details, raise an issue on <a href="https://github.com/ultralytics/yolov5/issues/new/choose">GitHub</a> for support, and join our <a href="https://discord.com/invite/ultralytics">Discord</a> community for questions and discussions!

To request an Enterprise License please complete the form at [Ultralytics Licensing](https://www.ultralytics.com/license).

# How to use
## 1. Local Deployment

### 1.1 Download the project locally

### 1.2 Configure the environment 

<pre> 
conda create -n yolov5 python=3.8.20 
conda activate yolov5 
pip install -r requirements.txt 
</pre>

## 2. Training and testing data configuration

## 2.1 Download the training data in YOLO format and create or modify a new ./data/dataset name.yaml

For example: 
<pre> 
train: /home/bxc/STOD/train/ImageName.txt (training data location) 
val: /home/bxc/STOD/val/ImageName.txt (validation data location) 
test: /home/bxc/STOD/val/ ImageName.txt (test data location) 
nc: 5 (total number of data categories) 
names: ['Small Vehicle', 'Large Vehicle', 'Ship', 'Airplane', 'Oil Tank'] (names of the data categories, corresponding in order) 
</pre>

## 3. Start Training

### 3.1 Configure data files

Modify behaviour 570 of train.py:

<pre> 
parser.add_argument("--data", type=str, default=ROOT / "data/dataset name.yaml", help="dataset.yaml path" 
</pre>

### 3.2 Changing Models

To replace the model with the original YOLOv5 model, modify line 569 of train.py (our model is models/yolov5-mask.yaml)

<pre> 
parser.add_argument("--cfg", type=str, default="models/yolov5.yaml", help="model.yaml path") 
</pre>

### 3.3 Modifying hyperparameters appropriately

### 3.4 Starting training

<pre> 
python train.py 
</pre>

### 3.5 End of training

The training file will be saved to ./run/train/project name folder.

## 4. Start testing

### 4.1 Configure the data file 
(if training is complete) Firstly, save the . /run/train/project name/weights to the folder: ./checkpoints

(If you don't want to train) you can download our trained ckp file directly from this project and save it to ./checkpoints

Modify the val.py file to configure the training data yaml and ckp file paths.

For example: 
<pre> 
parser.add_argument("--data", type=str, default=ROOT/ "data/STOD.yaml", help="dataset.yaml path") 
parser.add_argument("--weights ", nargs="+", type=str, default=ROOT/ "./checkpoints/best.pt", help="model path(s)") 
</pre>

### 4.4 Setting other hyperparameters

### 4.3 Starting the test 
<pre> 
python val.py 
</pre>

### 4.4 Completing the test

The test results will be saved to folder: ./run/val/project name
