# Facial Recognition Using Resnet50
Facial recognition is dond by genrating facial embeddings 
and then minimizing the distance between the facial embeddings 
the Concept of Siamese Networks is used to train the model.
The loss fuction used is Binary Cross Entropy 




***Siamese Network -
https://medium.com/wicds/face-recognition-using-siamese-networks-84d6f2e54ea4***

***Resnet50 -
https://towardsdatascience.com/the-annotated-resnet-50-a6c536034758***

# Prerequisites
It is advisable to create a separate python enviorment to install all packages
to avoid conflict 

<pre><code>pip install opencv-python
pip install tensorflow
pip install path
pip install torch
pip install scikit-learn</code></pre>


# Steps for Facial Recognition

**Step 1 - Facial Detection**



we will be using MTCNN for facial detetion 
to install mtcnn use the command 

<pre><code> pip install mtcnn </code></pre>
 
( Make sure you have the compatible version of opencv and tensorflow installed before intalling mtcnn 
 (if not mtcn will install opencv itself))

***MTCNN - https://towardsdatascience.com/face-detection-using-mtcnn-a-guide-for-face-extraction-with-a-focus-on-speed-c6d59f82d49***


**Step 2 - Facial Alignment**


MTCNN can perform facial alignment 


**Step 3 - facial recognition**

 # Training 
 The model is trained on the LFW dataset 
 ( make sure that you copy all the images in each of the folder - negative ,positive and anchor )
 
 ***In this model no pretrained weights are used and is made from scratch***

 # Dataset

 If you want to train on you whole dataset just remove .take() in the data pipline this will ensure the model takes input of the whole data. Though it is recomended only if you have GPU

# Prediction 
Finaly the model can predict the faces of people in real time 
