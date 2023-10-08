# yolov7_on_custom_dataset

#steps to make detection on custom dataset using yolov7
step 1: clone the repo of yolov7 using command "git clone https://github.com/WongKinYiu/yolov7"
step 2: install the necessary libraries
step 3: Ready dataset in Yolo format
step 4: download the weight 
step 5:train the model using command "python train.py --workers 8 --device 0 --batch-size 32 --data data/custom.yaml --img 640 640 --cfg cfg/training/yolov7-custom.yaml --weights 'yolov7_training.pt' --name yolov7-custom --hyp data/hyp.scratch.custom.yaml"
step 7: inference on image "python detect.py --weights yolov7.pt --conf 0.25 --img-size 640 --source inference/images/horses.jpg"
