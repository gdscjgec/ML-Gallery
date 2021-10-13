In this Repository, we are making Object Detection Program

Libraries Needed:
Numpy
argparse
cv2
To install these libraries run these commands in terminal:



`pip install numpy`

`pip install argparse`

`pip install cv2`


So, this Program Contains two subprogram
1st is Object Detection through Images and 2nd one is Real-time object detection which takes a live feed from the webcam of your device.
Both are using the pre-trained model in order to Work.

Object Detction through Given Images:


Real-Time Object Detection:

To initialize this Program we need a Pre-trained model so we are importing a list of class labels available in file MobilenetSSd.

To run this Program of Object_detction through images run this command:
python deep_learning_object_detection.py --image images/example_01.jpg --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel

To run real-time Object_detection make sure your webcam is connected and then run this command
python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel

Note: All other details are mentioned in the Code like how this Program works and its Tutorial
=======
![Screenshot 2021-10-11 102516](https://user-images.githubusercontent.com/55429956/136739104-0813bf51-57d1-46d4-8904-8df13b80e8d8.jpg)


Real-Time Object Detection:

![Screenshot 2021-10-11 102307](https://user-images.githubusercontent.com/55429956/136739107-43207051-f6f7-4363-9f1b-7368672f09b5.jpg)

To initialize this Program we need a Pre-trained model so we are importing a list of class labels available in file MobilenetSSd.

To run this Program of Object_detction through images run this command:
`python deep_learning_object_detection.py --image images/example_01.jpg --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel`

To run real-time Object_detection make sure your webcam is connected and then run this command
`python real_time_object_detection.py --prototxt MobileNetSSD_deploy.prototxt.txt --model MobileNetSSD_deploy.caffemodel`

Note: 
