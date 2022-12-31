![ALEX (1)](https://user-images.githubusercontent.com/71087332/210154655-5a9025f6-6cac-4bb6-9407-bdf3d0746718.png)

# Object Detection and Identification

Object detection is a computer technology related to computer vision and image processing that deals with detecting instances of semantic objects of a certain class (such as humans, buildings, or cars) in digital images and videos. Well-researched domains of object detection include face detection and pedestrian detection. Object detection has applications in many areas of computer vision, including image retrieval and video surveillance.

They are extensively used in computer vision tasks like image annotations, face recognition, face detection, object tracking, and many more. Not only that but they are also used to solve real-world problems like Automated CCTV surveillance where you can keep track of some objects that may cause some threats. Objects are tracked until any threat or abnormality is found. It can then be handled by recording the footage for a certain duration and alerting the respective authorities about it.

There are many methods to achieve Object Detection. Some of the methods used to achieve object detection are

    1.Single Shot MultiBox Detector (SSD)
    2.Faster R-CNN
    3.Histogram of Oriented Gradients (HOG)
    4.Region-based Convolutional Neural Network (R-CNN)
    5.YOLO (You Only Look Once)


## Deployment

We need to install anaconda and anaconda navigator.

![mpssss10](https://user-images.githubusercontent.com/71087332/210155547-418e2805-87d0-4e7a-91df-f03fe2453a19.PNG)

We are using jupyter notebook for code implementation.

![mpssss11](https://user-images.githubusercontent.com/71087332/210155556-825d2681-e1e6-49c2-aedd-8372d86f1434.PNG)

### Dependencies

    1.openCV
    2.matplotlib.pyplot


## Model and Algorithm

In this project we are using ***Tensorflow Frozen Model***
We are using ***ImageNet dataset*** for image identification
and we are using ***COCO dataset*** for image detection.

***Single Shot Detection algorithm*** is used in the project

## Single Shot Detection

Single Shot MultiBox Detector is a deep learning model used to detect objects in an image or from a video source. Single Shot Detector is a simple approach to solve the problem but it is very effective till now. SSD has two components and they are the Backbone Model and the SSD Head. Backbone Model is a pre-trained image classification network as a feature extractor. Usually, the fully connected classification layer is removed from the model. SSD Head is another set of convolutional layers added to this backbone and the outputs are interpreted as the bounding boxes and classes of objects in the spatial location of the final layer's activations.

Instead of using a traditional sliding window algorithm, SSD divides the image as grids, and each grid cell responsible for detecting objects in that region of the image. If there is no object detected then we output it as nothing or to be more precise we will put a “0” indicating that there is no object found.

What if there are many objects of the same instance in a single image. This is where Anchor Box comes into play. Anchor Boxes are simple boxes that are assigned with multiple anchors/prior boxes, which are predefined and have fixed size and shape within the grid cell. Based on this we are able to detect multiple objects in an image.

![image](https://user-images.githubusercontent.com/71087332/210155462-bb843461-63c9-4917-8b7a-6ef1aca658bb.png)

## Results

![image](https://user-images.githubusercontent.com/71087332/210155496-903d144f-b4db-496b-a607-b61c33c87167.png)

![image](https://user-images.githubusercontent.com/71087332/210155504-40b300ef-1ce0-4891-9855-66b7dd60b203.png)

![image](https://user-images.githubusercontent.com/71087332/210155508-73509823-7180-4aa1-a6da-224e4d0a24f0.png)

![image](https://user-images.githubusercontent.com/71087332/210155525-5e6f6a20-e8a2-479c-bd81-d8343d87829b.png)

## Conclusion

In this project, we are able to detect things the quickest by using SSD (single Shot Detector). It aids in the quickest identification of certain objects in the image. 
We may detect numerous objects simultaneously in real time by utilising Single Shot Multi-Box Detector. We have demonstrated how Real-Time Object Detection systems can make use of the widely utilised fully convolutional neural networks.
