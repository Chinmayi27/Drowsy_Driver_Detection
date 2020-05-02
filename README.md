# Drowsy_Driver_Detection
This is a project implementing Deep Learning concepts to detect drowsiness of a driver and sound an alarm if drowsy. It is built by real-time Eye-Tracking in videos.
Drowsy detection using OpenCV and Convolution Neural Networks.

## Requirements
*  Python 2.7
*  OpenCV
*  Keras
*  Tensorflow
*  Scipy

## Algorithm

Each eye is represented by 6 (x, y)-coordinates, starting at the left-corner of the eye (as if you were looking at the person), and then working clockwise around the eye.

## Download the dataset
you can download the dataset from the link given (http://parnec.nuaa.edu.cn/xtan/data/ClosedEyeDatabases.html)::
=>Download the dataset and put it in a folder named dataset
The dataset contains 4 folders namely:

* closedLeftEyes
* closedRightEyes
* openLeftEyes
* openRightEyes

## Training the data
```
    python eye_training.py
```

## Testing the drowsiness with webcam
~~~
    python drowsiness_predict.py
~~~

In the live web-cam it shows the time count of the closing of eyes and whether the driver opened or closed his eyes.
when the count becomes greater than 15 then the alarm will start ringing and tells the driver is Drowsy.

***Press Q*** to quit the web-cam
