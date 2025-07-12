After completing Inference Phase-1, the data is prepared and ready for the training process.
The data should contain the images, their labels and the classes.txt file.

#### Steps to train model
1.	Create a folder with name labelled_data.
2.	Create two folders in it with the names train and val.
3.	The train and val folders should contain images and labels folders.
4.	The ratio of images for the training and validation dataset is 70:30.
5.	The path of the dataset should be set in the train.yaml file.
The path is: 
gui_for_dlmodel\image-uploader\public\yolov5\data\train.yaml

```bash
# YOLOv5 🚀 by Ultralytics, AGPL-3.0 license
# COCO128 dataset https://www.kaggle.com/ultralytics/coco128 (first 128 images from COCO train2017) by Ultralytics
# Example usage: python train.py --data coco128.yaml
# parent
# ├── yolov5
# └── datasets
#     └── coco128  ← downloads here (7 MB)


# Train/val/test sets as 1) dir: path/to/imgs, 2) file: path/to/imgs.txt, or 3) list: [path/to/imgs1, path/to/imgs2, ..]
# path: ../datasets/coco128  # dataset root dir


train: data/train/images  # path to train images 
val: data/val/images  # path to validation images 
test:  # test images (optional)

# Classes
names:
  0: Person
  1: Bicycle
  2: Car
  3: Motorcycle
  4: Route Board
  5: Bus
  6: Commercial Vehicle
  7: Truck
  8: Traffic Sign
  9: Traffic Light
  10: Autorickshaw
  11: Tractor
  12: Ambulance
  13: Pushcart
  14: Construction Vehicle
  15: Animal
  16: Unmarked Speed Bump
  17: Marked Speed Bump
  18: Pothole
  19: Temporary Traffic Barrier
```
6.	To train the model, train.py should be executed.
The path is: gui_for_dlmodel\image-uploader\public\yolov5\train.py
The command to execute the train.py file is:
```bash
python3 train.py --data train.yaml --weights yolov5s.pt --epochs 200 --device 0
```
The training starts once this command is executed.
After the training is done, the path where the results get saved will be shown in the terminal.

