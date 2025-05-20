# Implementation-of-Erosion-and-Dilation

## Aim:
To implement Erosion and Dilation using Python and OpenCV.

## Software Required:
1. Anaconda - Python 3.7
2. OpenCV
   
## Algorithm:
### Step1:
Create a blank image.

### Step2:
Create a structuring element (5x5 rectangular)

### Step3:
Erode the image.

### Step4:
Dilate the image.

### Step5:
End the program.
 
## Program:

``` Python
# Import the necessary packages

import cv2
import numpy as np
from matplotlib import pyplot as plt

# Load the image

img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the Text using cv2.putText

# Create the text using cv2.putText
cv2.putText(img1,'Dharshini' ,(5,70),font,4,(255),2,cv2.LINE_AA)

# Create the structuring element

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(5,5))

# Erode the image

img_erode=cv2.erode(img1,kernel1)

# Dilate the image

img_dilate=cv2.dilate(img1,kernel1)
```
## Output:

### Display the input Image

![image](https://github.com/user-attachments/assets/29fc587b-5ecc-40b7-b8bb-d824d4346a21)

### Display the Eroded Image

![image](https://github.com/user-attachments/assets/83c35299-b6a2-4ca8-9819-5c44dfc49f05)

### Display the Dilated Image

![image](https://github.com/user-attachments/assets/1f02a026-84b3-4830-89fc-34448cb08c7c)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
