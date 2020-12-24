# classification-of-covid19-using-chest-xray-images-in-keras


Goals:
======
* Build and Train the Convolutional Neural Network using Keras with Tensorflow as Backend
* Visualize Data in Matplotlib
* Make use of the Trained Model to Predict on a New Set of Data

Project Steps:
======
1. Introduction & Import Libraries
2. Clone and Explore Dataset 
3. Data Visualization
4. Data preprocessing and Augmentation
5. Build a Convolutional Neural Network (CNN)
6. Compile and Train the Model
7. Performance Evaluation
8. Prediction on New Data


Convolutional Neural Network Model Details:
========

Model: "sequential"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d (Conv2D)              (None, 150, 150, 32)      2432      
_________________________________________________________________
max_pooling2d (MaxPooling2D) (None, 75, 75, 32)        0         
_________________________________________________________________
dropout (Dropout)            (None, 75, 75, 32)        0         
_________________________________________________________________
conv2d_1 (Conv2D)            (None, 75, 75, 64)        51264     
_________________________________________________________________
max_pooling2d_1 (MaxPooling2 (None, 37, 37, 64)        0         
_________________________________________________________________
dropout_1 (Dropout)          (None, 37, 37, 64)        0         
_________________________________________________________________
flatten (Flatten)            (None, 87616)             0         
_________________________________________________________________
dense (Dense)                (None, 256)               22429952  
_________________________________________________________________
dropout_2 (Dropout)          (None, 256)               0         
_________________________________________________________________
dense_1 (Dense)              (None, 1)                 257       
=================================================================
Total params: 22,483,905
Trainable params: 22,483,905
Non-trainable params: 0
