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
    -Size: 
         The orginal dataset had more than 30,000 retina images but for this repository we have used 2929 for training and 733 images where used for Testing

# Data Visualization
count plot for all classes (diagnosis) in the dataset
<img width="392" alt="image" src="https://user-images.githubusercontent.com/89664911/171306832-16bf7d0f-b2f7-408e-88b8-f9267a015c5d.png">
Visualization of the retina images along with their diagnosis. The images are taken using different type of camera under different lighting condition so they look different. The images are also taken from both left and right side for each patients. The difference in the angle where it was taken can be seen from the picture. 
<img width="593" alt="image" src="https://user-images.githubusercontent.com/89664911/171325918-dbab3f11-52e2-487c-9592-15b7dbdf265d.png">

# Problem Formulation and Training
The dataset was shuffled and spilit to training and Test. Then run-time augmentation was done on both set. For training datagenerator,  normalization, shear angle, zooming range and horizontal flip was added. But for test just normalization was added.Then datagenerator is created for training, validation and test dataset.Next the Deep learning model was compiled and Trained.Early stopping was used to exit training when validation loss was not decreasing  after certain epochs.The the best model with lower validation loss was saved.
<img width="391" alt="image" src="https://user-images.githubusercontent.com/89664911/171328894-619fea27-1e87-4814-bde7-b4163045f56f.png">

# Performance Comparison
The accuracy score of the model was found to be 0.82947. The images were visualized inorder to see the original diagnosis and the predict diagnosis. For most cases the model predicted the orginal diagnosis.
<img width="272" alt="image" src="https://user-images.githubusercontent.com/89664911/171331189-bbfe82df-7333-4ae6-83d7-161e8faefbdf.png">
<img width="271" alt="image" src="https://user-images.githubusercontent.com/89664911/171331248-11bdecb1-b0a2-4158-a2df-c6a4c9867d77.png">
<img width="273" alt="image" src="https://user-images.githubusercontent.com/89664911/171331306-6c23e872-c2cc-421c-9683-d39eba4bc0d4.png">
<img width="272" alt="image" src="https://user-images.githubusercontent.com/89664911/171331370-11d01fa2-2347-42aa-8543-cc1b2a7e5a7b.png">
# Conclusions

Based on this dataset using Residual Neural network is good for the classification of images since the model had high accuracy point.

# Future work






      
