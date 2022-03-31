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
### Developed By: Dhanasekar G
### Register Number: 212220230009
i) #To Read,display the image
```
import cv2
img = cv2.imread('bike.jpg',1)
cv2.imshow('dhans',img)
cv2.waitKey(0)

```
ii) #To write the image
```

cv2.imwrite('ds.jpg',img)

```
iii) #Find the shape of the Image
```
print(img.shape)



```
iv) #To access rows and columns
```

ds = cv2.imread('tony.jpg',1)
import random
for i in range(70):
    for j in range(ds.shape[1]):
        ds[i][j]= [random.randint(0,255),random.randint(0,255),random.randint(0,255)]
cv2.imshow('image',ds)
cv2.waitKey(0)

```
v) #To cut and paste portion of image
```

bw2=cv2.imread('ronaldo.jpg',1)
tag=bw2[30:100,30:120]
bw2[50:120,100:190]=tag
cv2.imshow("cutting portion",bw2)
cv2.waitKey(0)
cv2.destroyAllWindows()




```

## Output:

### i) Read and display the image


![1](https://user-images.githubusercontent.com/75264748/161105629-e4491581-d298-444a-a0f6-7d283ebdb5b3.png)


### ii)Write the image
![2](https://user-images.githubusercontent.com/75264748/161105664-1c34a314-fc65-4a2e-a22b-a8daf19d787c.png)


### iii)Shape of the Image
![2](https://user-images.githubusercontent.com/75264748/161105679-c4559ec6-eb1c-4a36-9efc-8908ca6f9ea3.png)


### iv)Access rows and columns

![3](https://user-images.githubusercontent.com/75264748/161105748-3cb75a27-0de0-4ad2-a303-eb7f67c5dc40.png)

### v)Cut and paste portion of image

![4](https://user-images.githubusercontent.com/75264748/161105769-7ac33fb3-ce9c-4fb0-a674-730eea0f215d.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


