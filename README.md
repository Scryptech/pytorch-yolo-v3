# A PyTorch implementation of a YOLO v3 Object Detector

[UPDATE] : This repo serves as a driver code for my research. I just graduated college, and am very busy looking for research internship / fellowship roles before eventually applying for a masters. I won't have the time to look into issues for the time being. Thank you.


This repository contains code for a object detector based on [YOLOv3: An Incremental Improvement](https://pjreddie.com/media/files/papers/YOLOv3.pdf), implementedin PyTorch. The code is based on the official code of [YOLO v3](https://github.com/pjreddie/darknet), as well as a PyTorch 
port of the original code, by [marvis](https://github.com/marvis/pytorch-yolo2). One of the goals of this code is to improve
upon the original port by removing redundant parts of the code (The official code is basically a fully blown deep learning 
library, and includes stuff like sequence models, which are not used in YOLO). I've also tried to keep the code minimal, and 
document it as well as I can. 

##How To prepare the inviroment and run the program
-install anaconda3 (a virtual inviroment python manager) https://www.anaconda.com/
-create the enviroment by typing: conda env create -f pytorch.yml
-put the weights file in the root of the folder and name it as yolov3.weights
-rename your cfg file to yolov3.cfg inside the cfg folder
-put the names in coco.names file under data folder
-in detect.py change the number of classes to the number of names in coco.names
-run : python detect.py




