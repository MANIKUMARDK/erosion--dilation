# Reg.No:212223230121
# Name: Mani Kumar DK
# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
### Algorithm:
#### Step1:<br>
Import the necessary pacakages

#### Step2:<br>
Create the text using cv2.putText

#### Step3:<br>
Create the structuring element

#### Step4:<br>
Erode the image


#### Step5: <br>
Dilate the Image

 
## Program:

# Import the necessary packages
````
import cv2
import numpy as np
import matplotlib.pyplot as plt
````

# Create the Text using cv2.putText
````
def load_img():
    blank_img=np.zeros((600,600))
    font=cv2.FONT_HERSHEY_SIMPLEX
    cv2.putText(blank_img,"MANI KUMAR",(50,300),fontFace=font,fontScale=5,color=[255,255,255],thickness=25,lineType=cv2.LINE_AA)
    return blank_img
````


# Create the structuring element
````
image = load_img()
plt.imshow(image, cmap='gray')
plt.show()
````

# Erode the image
````
kernel=np.ones((5,5),np.uint8)
kernel
ersion=cv2.erode(image,kernel,iterations=4)
plt.imshow(ersion,cmap='gray')
````

# Dilate the image
````
dilution=cv2.dilate(image,kernel,iterations=4)
plt.imshow(dilution,cmap='gray')
````



## Output:

### Display the input Image

<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/49cfe567-adec-4c8b-a106-39d671783902" />



### Display the Eroded Image

<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/f944fefb-2479-43b5-a447-9903ba7b55c4" />

### Display the Dilated Image


<img width="425" height="418" alt="image" src="https://github.com/user-attachments/assets/a61f93ac-7b9a-4f17-b331-7219d925e5ca" />

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
