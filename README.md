# Faceoff
__FaceOff__ is a Computer Vision Model that was built using OpenCV and deployed onto a Webpage using Streamlit and hosted via Heroku. 

__Step 1:__ Create a dataset of all the images. To do this, we import opencv library. Remember we use the opencv-contrib-python library as it contains all the main modules as well as the contributed/extra modules. 

__About the OpenCV library:__

OpenCV (Open Source Computer Vision Library) is an open source computer vision and machine learning software library. OpenCV was built to provide a common infrastructure for computer vision applications and to accelerate the use of machine perception in the commercial products. Being a BSD-licensed product, OpenCV makes it easy for businesses to utilize and modify the code.

![alt text](https://miro.medium.com/max/1050/1*uICHe7Ul2F3rBim1a7GQaA.png)

Next, we use the Haarcascade Face Classifier to detect faces in the images supplied. 

__About Haar cascades:__
Haar cascades, first introduced by Viola and Jones in their seminal 2001 publication, Rapid Object Detection using a Boosted Cascade of Simple Features, are arguably OpenCV’s most popular object detection algorithm.Sure, many algorithms are more accurate than Haar cascades (HOG + Linear SVM, SSDs, Faster R-CNN, YOLO, to name a few), but they are still relevant and useful today.One of the primary benefits of Haar cascades is that they are just so fast — it’s hard to beat their speed.
The downside to Haar cascades is that they tend to be prone to false-positive detections, require parameter tuning when being applied for inference/detection, and just, in general, are not as accurate as the more “modern” algorithms we have today.

That said, Haar cascades are:
1. An important part of the computer vision and image processing literature
2. Still used with OpenCV
3. Still useful, particularly when working in resource-constrained devices when we cannot afford to use more computationally expensive object detectors

__Step 2:__ Is to train the image dataset using the LBPH (Local Binary Pattern Histogram) face recognition algorithm.

![alt text](https://miro.medium.com/max/1838/1*-cyqWPcas3CXp4O2O7xPpg.png)

__Step 3:__ We finally use the Haar cascades to detect and then LBPH algorithm to recognize faces in the provided image with that to our stored data. If it matches, we get the name of the individual! 

Access the Heroku App from this link https://faceoff-by-darthvardaan.herokuapp.com/ 

