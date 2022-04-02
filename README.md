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
### Developed By: S.Sumyuktha Rani
### Register Number: 212220230050
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('scenery.jpg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```
cv2.imwrite('apple.jpg',color_image)
cv2.imshow('apple',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
iii) #Find the shape of the Image
```
import cv2
color_image=cv2.imread('scenery.jpg',-1)
print(color_image.shape)

```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('scenery.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230050, S.Sumyuktha Rani',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
v) #To cut and paste portion of image
```
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('panda',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```

## Output:

### i) Read and display the image
![sum](https://user-images.githubusercontent.com/75235818/161392904-15c83055-cadd-4fb2-a123-698f1a8c560d.jpg)

### ii)Write the image
![apple](https://user-images.githubusercontent.com/75235818/161392921-cd59f3ca-12c2-4290-a2b8-fd5a27d0b783.jpg)

### iii)Shape of the Image
![shape](https://user-images.githubusercontent.com/75235818/161392932-0ec01414-9800-4af2-96ed-aa133c24e620.jpg)

### iv)Access rows and columns
![rows_and_cols](https://user-images.githubusercontent.com/75235818/161392945-78cc0f31-0b96-4b7a-a9c1-4d36cbd4b88e.jpg)

### v)Cut and paste portion of image
![sliced_image](https://user-images.githubusercontent.com/75235818/161392980-63c6fc2e-5846-48ac-b324-2ab07e36b569.jpg)

## Result:
Thus the images are read, displayed, and written successfully using the python program.


