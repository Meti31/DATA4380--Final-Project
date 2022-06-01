<img width="199" alt="image" src="https://user-images.githubusercontent.com/89664911/171169741-90a0c49a-aa59-4430-891f-c55428f85ff6.png">

#  Diabetic Retinopathy Detection Using Residual Neural Network
 
 This repository holds an attempt to apply ResNet to Retina Images to Detect Diabetic Retinopathy using data from "Diabetic Retinopathy Detection" Challenge https://www.kaggle.com/c/diabetic-retinopathy-detection" 
 
 #  Overview
 
  The dataset have a large set of high-resolution retina images taken under a variety of imaging conditions. A left and right field is provided for every subject. Images are labeled with a subject id as well as either left or right 
A clinician has rated the presence of diabetic retinopathy in each image on a scale of 0 to 4, according to the following scale:

0 - No DR
1 - Mild
2 - Moderate
3 - Severe
4 - Proliferative DR

The task is  to create an automated analysis system capable of assigning a score based on this scale.
In this repository ResNet is used to try to classfiy the retina images into the scale above.
The model had an accuracy score of 0.82947

# Summary of Workdone

Data:
    
    Type:
    Input: retina images taken by from different models and types of cameras. And the images are different size. And there is a csv file that contains the diagnosis along with id_code of the images
    Size: 
     The orginal dataset had more than 30,000 retina images but for this repository we have used 2929 for training and 733 images where used for Testing

# Data Visualization
<img width="392" alt="image" src="https://user-images.githubusercontent.com/89664911/171306832-16bf7d0f-b2f7-408e-88b8-f9267a015c5d.png">

      
