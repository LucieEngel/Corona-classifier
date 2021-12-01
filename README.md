# Detect pnemonia from chest X-Rays 

The aim of this notebook is to develop a machine learning model to classify chest X-rays between healthy patients and patients with pnemonia. 

Author : Lucie Engel

## Dataset 

I am using the open source dataset "CoronaHack - Chest X-Ray" from kaggle that can be found here : https://www.kaggle.com/praveengovi/coronahack-chest-xraydataset

The dataset is structered this way :

## Transfer learning ResNet50

My first intuition was to use transfer learning with a pre-trained ResNet50 on the ImageNet dataset. The training phase appeared to be very unstable even with low learning rate. 

## 
For this reason, I am currently working on a much smaller CNN. Our AUC for the testing set is approximately equal to 


