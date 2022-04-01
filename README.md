# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:
### Register Number: 
i) #To Read,display the image
```
import cv2
img =cv2.imread('bird.jpg',1)
cv2.imshow('bird',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
ii) #To write the image
```
cv2.imwrite('img.jpg',img)
cv2.destroyAllWindows()
```
iii) #Find the shape of the Image
```python3
print(img.shape)
```
iv) #To access rows and columns
```python3
import random
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('image',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
v) #To cut and paste portion of image
```python3
import cv2
img=cv2.imread('bird.jpg',1)
tag=img[50:70,50:70]
img[100:120,100:120]=tag
cv2.imshow('image',img)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

## Output:

### i) Read and display the image
![output](oprs.png)

### ii)Write the image
![output](opw.png)

### iii)Shape of the Image
![output](opshape.png)

### iv)Access rows and columns
![output](opaccess.png)

### v)Cut and paste portion of image
![output](opcp.png)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


