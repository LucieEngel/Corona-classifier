# Detect pnemonia from chest X-Rays 

The aim of this notebook is to develop a machine learning model to classify chest X-rays between healthy patients and patients with pnemonia. 

Author : Lucie Engel

## Dataset 

I am using the open source dataset "CoronaHack - Chest X-Ray" from kaggle that can be found here : https://www.kaggle.com/praveengovi/coronahack-chest-xraydataset

The dataset is structered this way : the X-rays are saved in the folder "Coronahack-Chest-XRay-Dataset" and divided between the training set and the testing set. The mapping between filenames and classes (Pnemionia, Normal) is stored in the csv file "Chest_xray_Corona_Metadata.csv". 

## Transfer learning ResNet50

My first intuition was to use transfer learning with a pre-trained ResNet50 on the ImageNet dataset. The training phase appeared to be very unstable even with low learning rate, which led me to choose a much smaller model afterwards. 
Using a ResNet50 pre-trained on ImageNet can be questionnable too. It could be interesting to find out if a pre-trained ResNet50 on a medical imaging dataset exists. 

## Shallow CNN 

I am currently working on a much smaller CNN (only 895,579 trainable parameters compared to the 24,845,333 trainable parameters for the first model). Our AUC for the testing set is approximately equal to 88%. 

## References 

* [Covid-19 Detection from Lung X-rays](https://www.kaggle.com/sidharthavs/covid-19-detection-from-lung-x-rays)
* [Computer Vision course from Kaggle](https://www.kaggle.com/learn/computer-vision)




