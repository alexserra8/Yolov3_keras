# Yolov3_keras

In this respository there are two Jupyter Notebooks which define the YoloV3 network in Keras. This is repository can be used to train or test the YoloV3.

- "Definicion del modelo" --> is the main *.ipynb where the YoloV3 is fully defined. Perfect for training the model.

- "Funciones Yolo" --> a reduced *.ipynb where there are only the functions you will need to run to start your model once you have it trained.


### BeforeTrain

Furthermore, there is a folder called "BeforeTrain" where you can find two Jupyter Notebooks which can helps to create more data (Data augmentation) and helps you to split data between training and validation:

    · "Distorsionar Fotos" --> We apply data augmentation using GAUSSIAN NOISE. Also, a code is written to obtain also the new bounding boxes we are obtaining in format *.txt that Yolo require.

    · "ExtractText_Train_Valid" --> In this notebook, once we have all the images, we split them in training and validation data. We obtain two files in format *.txt, one where there are the locations of training images, and the other with the locations of the validation images. This is the format required for Yolo.
    

### Applications

In this folder we show an applications where we can obtain if an object or product that appears in the video is moving to the right or to the left. We used this code to detect if a product of a supermarket is entring to the shopping cart or leaving. We have 3 versions:

**IMPORANT**: _the notebook "FuncionesYolo" has to be in the same directory to run it._

* Leer definitivo1 --> First document where we achieve obtain the bounding box of several photograms of the video (C=30 means that we take one photo every second of the video, C=15 means we take a phot of the video every 0,5 seconds). Here we don't detect the direction of the object

* Leer definitivo2 --> Based on "Leer definitivo1", we coded one version for detecting the detection of the product.

* Leer definitivo3 --> Based on "Leer definitivo2", the newest version of the code. We recommend use this version.
