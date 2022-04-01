# Diabetic_Retinopathy_Competition

A DL classification project to detect Diabetic Retinopathy using transfer learning techniques

# Description of Dataset

### [APTOS 2019 Blindness Detection](https://www.kaggle.com/competitions/aptos2019-blindness-detection/data)

A clinician has rated each image for the severity of diabetic retinopathy on a scale of 0 to 4:

1.  No DR (0)
2.  Mild (1)
3.  Moderate (2)
4.  Severe (3)
5.  Proliferative DR (4)


Like any real-world data set, you will encounter noise in both the images and labels. Images may contain artifacts, be out of focus, underexposed, or overexposed. The images were gathered from multiple clinics using a variety of cameras over an extended period of time, which will introduce further variation.

#	Preprocessing

Preprocessing is inspired from the https://www.kaggle.com/code/ratthachat/aptos-eye-preprocessing-in-diabetic-retinopathy

![Preview of Dataset](https://github.com/tshr-d-dragon/Diabetic_Retinopathy_Competition/blob/main/download.png)

# Augmentation

To handle imbalance dataset, performed following augmentations using [Albumentations](https://albumentations.ai/docs/) library

1.  HorizontalFlip
2.  VerticalFlip
3.  VerticalHorizontalFlip
4.  RandomContrast
5.  RandomBrightness
6.  RandomBrightnessContrast
7.  GridDistortion
8.  RandomBrightnessContrast+GridDistortion

# Training

1.  Trained pretrained EfficientNetB0, Inception_ResNetV2, DenseNet121 and Xception models for both the dataset. 
2.  The training notebooks are present in ***Models*** folder.
3.  History details of all of the models are present in ***History*** folder



##### For better performance, we can train models for more epochs and balanced dataset will be needed for the same.
