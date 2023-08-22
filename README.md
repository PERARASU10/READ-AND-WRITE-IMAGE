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
### Developed By: PERARASU M
### Register Number: 212222100033
i) #To Read,display the image
```
  import cv2
color_img=cv2.imread('ben10.jpg',1)
cv2.imshow('212222100033_PERARASU',color_img)
cv2.waitKey(0)  

```
ii) #To write the image
```
import cv2
color_img=cv2.imread('ben10.jpg',1)
w=cv2.imwrite('1.png',color_img)
cv2.imshow('212222100033_PERARASU',color_img)
cv2.waitKey(0) 


```
iii) #Find the shape of the Image
```
import cv2
import random
color_img=cv2.imread('ben10.jpg',1)
print(color_img.shape)

```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('ben10.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('212222100033_PERARASU',color_img)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('ben10.jpg',-1)
tag=color_image[300:400,300:400]
color_image[50:150,50:150]=tag
cv2.imshow('212222100033_PERARASU',color_image)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image


![image](https://github.com/PERARASU10/READ-AND-WRITE-IMAGE/assets/118348589/794d3914-0660-4b82-9d17-98886b180c46)




### ii)Write the image


![image](https://github.com/PERARASU10/READ-AND-WRITE-IMAGE/assets/118348589/da3fdd60-d1e6-4a56-bc7d-0d1f6ca6f027)


### iii)Shape of the Image


![image](https://github.com/PERARASU10/READ-AND-WRITE-IMAGE/assets/118348589/2e122cef-374e-417f-a81b-8a91e6487f7a)



### iv)Access rows and columns


![image](https://github.com/PERARASU10/READ-AND-WRITE-IMAGE/assets/118348589/011684e1-eae7-4236-8b1c-7774fc4edc11)



### v)Cut and paste portion of image

![image](https://github.com/PERARASU10/READ-AND-WRITE-IMAGE/assets/118348589/8d34d286-000a-484e-8c59-e4e581a1bd9f)



## Result:
Thus the images are read, displayed, and written successfully using the python program.
