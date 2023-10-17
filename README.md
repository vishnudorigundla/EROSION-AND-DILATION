# EROSION-AND-DILATION

## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import cv2 and numpy packages.
### Step2:
Create the text using cv2.putText() and show the Imge containing Text.
### Step3:
Create the structuring element using cv2.getStructuralElement().

### Step4:
Using structuring element erode the image.

### Step5:
Usig structuring element dilate the image.

### Step6:
Show the Erroded and Dilated Images with Original Image.
## Program:

``` Python
Developed by: D.vishnu vardhan reddy
Register Number: 212221230023
# Import the necessary packages
import cv2
import numpy as np
img1= np.zeros((350,1400),dtype ='uint8')
# Create the Text using cv2.putText
font=cv2.FONT_HERSHEY_SCRIPT_SIMPLEX
cv2.putText(img1,'vishnu',(5,50),font,2,(255),3,cv2.LINE_AA)
cv2.imshow('My Image',img1)

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_ELLIPSE,(7,7))

# Erode the image
erodeimg=cv2.erode(img1,kernel1)
cv2.imshow("Eroded Image",erodeimg)

# Dilate the image
dilateimg=cv2.dilate(img1,kernel1)
cv2.imshow("Dilated Image",dilateimg)


```
## Output:

### Display the input Image
![image](https://github.com/vishnudorigundla/EROSION-AND-DILATION/assets/94175324/34d9cc5e-d389-4d70-b8ed-78f9261a18ba)

### Display the Eroded Image
![image](https://github.com/vishnudorigundla/EROSION-AND-DILATION/assets/94175324/9e8e5413-5242-4520-a8b0-f381c3fac0ae)

### Display the Dilated Image
![image](https://github.com/vishnudorigundla/EROSION-AND-DILATION/assets/94175324/ae87dc38-7a69-4d99-8f70-0371c2c76df3)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
