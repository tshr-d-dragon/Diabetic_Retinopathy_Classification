# Diabetic_Retinopathy_Competition

A DL classification project to detect Diabetic Retinopathy using transfer learning techniques

# Description of Dataset

### [APTOS 2019 Blindness Detection](https://www.kaggle.com/competitions/aptos2019-blindness-detection/data)

A clinician has rated each image for the severity of diabetic retinopathy on a scale of 0 to 4:

0 - No DR
1 - Mild
2 - Moderate
3 - Severe
4 - Proliferative DR

Like any real-world data set, you will encounter noise in both the images and labels. Images may contain artifacts, be out of focus, underexposed, or overexposed. The images were gathered from multiple clinics using a variety of cameras over an extended period of time, which will introduce further variation.

#	Preprocessing

Preprocessing is inspired from the https://www.kaggle.com/code/ratthachat/aptos-eye-preprocessing-in-diabetic-retinopathy

![Preview of Dataset](https://github.com/tshr-d-dragon/Diabetic_Retinopathy_Classification/blob/main/download.png)

# Augmentation

To handle imbalance dataset, performed following augmentations using Albumentations library
a.	HorizontalFlip
b.	VerticalFlip
c.	VerticalHorizontalFlip
d.	RandomContrast
e.	GridDistortion
f.	ElasticTransform
g.	RandomBrightness
h.	ShiftScaleRotat
