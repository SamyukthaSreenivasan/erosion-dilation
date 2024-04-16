# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText
### Step3:
Create the structuring element
### Step4:
Erode the image
### Step5:
Dilate the image 
## Program:
```
Developed By:Samyuktha S
Register Number:212222240089
```
# Erode the image
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'TheAILearner',(5,70),font,2,(255),5,cv2.LINE_AA)
k=np.ones((5,5),np.uint8)
k1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_erode1=cv2.erode(img,k1)
plt.imshow(image_erode1)
plt.axis('off')
```
# Dilate the image
```
k=np.ones((5,5),np.uint8)
k1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))
image_dilate1=cv2.dilate(img,k1)
plt.imshow(image_dilate1)
plt.axis('off')
```
## Output:

### Display the Eroded Image
![image](https://github.com/SamyukthaSreenivasan/erosion-dilation/assets/119475703/2a40dc18-23b6-4ae5-b37f-8875fee63958)

### Display the Dilated Image
![image](https://github.com/SamyukthaSreenivasan/erosion-dilation/assets/119475703/8cd22b75-30d4-4822-abd3-fc3460ad28d5)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
