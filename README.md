# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: PRAKASH M
Register NO: 212222100035
```
``` Python
# Import the necessary packages
import cv2
import numpy as np



# Create the Text using cv2.putText
img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'JEEVA ABISHAKE A',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()



# Create the structuring element
struct_ele= np.ones((9,9),np.uint8)



# Use Opening operation
opening = cv2.morphologyEx(img,cv2.MORPH_OPEN,struct_ele)
cv2.imshow('Opening',opening)
cv2.waitKey(0)
cv2.destroyAllWindows()




# Use Closing Operation
closing = cv2.morphologyEx(img,cv2.MORPH_CLOSE,struct_ele)
cv2.imshow('Closing',closing)
cv2.waitKey(0)
cv2.destroyAllWindows()




```
## Output:

### Display the input Image
![WhatsApp Image 2023-10-11 at 16 17 58](https://github.com/Prakashmathi2004/OPENING--CLOSING/assets/118350045/f906d492-d2e3-48b8-835f-3e45cfb567f5)



### Display the result of the Opening
![WhatsApp Image 2023-10-11 at 16 18 40](https://github.com/Prakashmathi2004/OPENING--CLOSING/assets/118350045/9c89b012-3f0e-4e58-a32a-c2f65e22ca2f)


### Display the result of Closing
![WhatsApp Image 2023-10-11 at 16 19 20](https://github.com/Prakashmathi2004/OPENING--CLOSING/assets/118350045/7a17f4c9-3cd5-411a-89c4-b888881835d6)



## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
