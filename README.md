# Face mask detection using YOLOv3 in tensorflow
## Results:
![Face mask detection result image](/results/z4.jpg)
![Face mask detection result image](/results/z5.jpg)
![Face mask detection result image](/results/z3.jpg)<br/><br/>
You can check other results in results folder.<br/>
## Dataset:
Dataset can be found here-> [drive link](https://drive.google.com/drive/folders/1pAxEBmfYLoVtZQlBT3doxmesAO7n3ES1?usp=sharing) <br/>
The dataset is composed by MAFA, WIDER FACE and various other datasets.<br/>
Annotations of training and validation set is available in madel_data folder in YOLO format.
## Pre trained Weights:
If you do not wish to train weights from scratch. Here are the weights I obtained after training for decent amount of time -> 
[weights](https://drive.google.com/file/d/1-BL5nkVSjwBxOpDbTzBWOIHn8I-HopaF/view?usp=sharing)<br/> 
## Training Weights:
For training from scratch, download pretrained weights on COCO dataset from [here](https://pjreddie.com/media/files/yolov3.weights) and paste it in model_data folder. Then, 
run the following bash command to convert the weights from darknet format to Keras format(.h5 format):
```bash
python convert.py model_data/yolov3.cfg model_data/yolov3.weights model_data/yolo_weights.h5
```
and start training.
