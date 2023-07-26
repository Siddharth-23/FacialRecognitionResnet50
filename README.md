# FacialRecognitionResnet50

# Steps for Facial Recognition

Step 1 - Facial Detection 

we will be using MTCNN for facial detetion 

Step 2 - Facial Alignment 

MTCNN can perform facial alignment 

Step 3 - facial recognition

# Working of the project 

Image is taken from the user and facial embeddings are calculated using the Resnet50. 
Through simamese Networks the facial embedings are evaluated 
 Siamese Network -
 https://medium.com/wicds/face-recognition-using-siamese-networks-84d6f2e54ea4

 # Training 
 The model is trained on the LFW dataset ( make sure that you copy all the images in each of the folder - negative ,positive and anchor )
 In this model no pretrained weights are used and is made from scratch

 # dataset

 If you want to train on you whole dataset just remove .take() in the data pipline this will ensure the model takes input of the whole data. Though it is recomended only if you have GPU 

# Prediction 
Finaly the model can predict the faces of people in real time 
