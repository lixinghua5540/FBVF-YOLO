# Introduction of RS-STOD

RS-STOD Small Target Detection Dataset (for Remote Sensing Tasks) 

The dataset used in this project is specially designed for the task of small target detection in remote sensing imagery, covering a wide range of small-scale target types, which is suitable for the training and evaluation of target detection models, especially for small target recognition scenarios in dense distribution, low contrast and occlusion situations.

Note: A small target is defined as a bbox with the longest side less than 32 pixels, and an ultra-tiny target is defined as a bbox with the longest side less than 16 pixels.

![image](https://github.com/lixinghua5540/FBVF-YOLO/blob/master/RS-STOD/images/Dataset_images.jpg)
<p align="center">Dataset annotation<p>

![image](https://github.com/lixinghua5540/FBVF-YOLO/blob/master/RS-STOD/images/Percentage%20of%20each%20category.jpg)
<p align="center">Instance size of RS-STOD<p>

![image](https://github.com/lixinghua5540/FBVF-YOLO/blob/master/RS-STOD/images/RS-STOD%20labelling%20details.jpg)
<p align="center">Instance detail information for RS-STOD<p>


## 📦 Dataset contents 

This dataset contains two annotation formats: the YOLO format and the COCO format, which are placed in folders with corresponding names.

The coco format is divided into train and val, and the YOLO format is not divided.

### yolo

For storing images in yolo format and labelling txt

### coco

For storing images in coco format and labelling json

### classes.txt

list of category names, one category name per line, corresponding to category_id in COCO.

### For more details of RS-STOD, see our paper: A front-back view fusion strategy and a novel dataset for super tiny object detection in remote sensing imagery

## 🔗 Download link 

The full dataset has been uploaded to 

📎 Link: https://pan.baidu.com/s/1jO7W3mQ07Ec0xHcnTC0ANg?pwd=2u3z 

🔑 Extract code: 2u3z 

## ⚠️ Please use the dataset appropriately for scientific purposes only, commercial use or redistribution is prohibited!


## 📄 Citation Format 

If you have used this dataset in your research, please cite it in the following format:

<pre> bibtex 
 @article{BAI2025114051, 
 title = {A front-back view fusion strategy and a novel dataset for super tiny object detection in remote sensing imagery}, 
 author = {Xuechen Bai and Xinghua Li and Jianhao Miao and Huanfeng Shen}, 
 journal = {Knowledge-Based Systems}, 
 volume = {326}, 
 pages = {114051} , 
 year = {2025}, 
 doi = {https://doi.org/10.1016/j.knosys.2025.114051}, 
 } </pre>
 
