# Yolov3_keras

In my final project of Master Data Science I developed a prototype of Smark. This project implement an intelligent shopping cart equipped with a camera that, applying artificial vision techniques, automatically recognizing the products that are introduced to it.

In this repository I will show my work, and I encourage you to try it on your own with you data. I used **Python 3.**

I have upload 3 folders:

* **BeforeTrain**: where you can find a few helpful codes for Data agumentation and Split train and validation data.

* **Keras**: in this folder there is the structure of YoloV3 written in keras.

* **Applications**: here there are differents codes that will detect if the object is moving to the right or to the left.

* **Data**: where you can find a few images of the data for try it. And there is the weight of my CNN if you want to reply the project (train this weight took me more than 4 days :P)

* **Results**: I share a video and photos with the results.




### BeforeTrain

Furthermore, there is a folder called "BeforeTrain" where you can find two Jupyter Notebooks which can helps to create more data (Data augmentation) and helps you to split data between training and validation:

* "Distorsionar Fotos" --> We apply data augmentation using GAUSSIAN NOISE. Also, a code is written to obtain also the new bounding boxes we are obtaining in format *.txt that Yolo require.

* "ExtractText_Train_Valid" --> In this notebook, once we have all the images, we split them in training and validation data. We obtain two files in format *.txt, one where there are the locations of training images, and the other with the locations of the validation images. This is the format required for Yolo.
   
   
   

### Applications

In this folder we show an applications where we can obtain if an object or product that appears in the video is moving to the right or to the left. We used this code to detect if a product of a supermarket is entring to the shopping cart or leaving. We have 3 versions:

**IMPORANT**: _the notebook "FuncionesYolo" has to be in the same directory to run it._

* Leer definitivo1 --> First document where we achieve obtain the bounding box of several photograms of the video (C=30 means that we take one photo every second of the video, C=15 means we take a phot of the video every 0,5 seconds). Here we don't detect the direction of the object

* Leer definitivo2 --> Based on "Leer definitivo1", we coded one version for detecting the detection of the product.

* Leer definitivo3 --> Based on "Leer definitivo2", the newest version of the code. We recommend use this version.


If you have any doubt, contact me and I will be glad to help :)
