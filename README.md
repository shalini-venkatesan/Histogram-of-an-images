# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().



### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
```python
# Developed By: Shalini V
# Register Number: 212222240096
```
### Read image
```
import cv2
import matplotlib.pyplot as plt
Gray_image = cv2.imread('i11.jpg')
Color_image = cv2.imread('i22.jpg')
plt.imshow(Gray_image)
plt.show()
plt.imshow(Color_image)
plt.show()
```
### Calculate Hist
```
hist = cv2.calcHist([Gray_image],[0],None,[256],[0,256])
hist1 = cv2.calcHist([Color_image],[1],None,[256],[0,256])

```
### Histogram for gray image
```
plt.figure()
plt.title("Histogram")
plt.xlabel('grayscale value')
plt.ylabel('pixel count')
plt.stem(hist)
plt.show()
```
### Histogram for color image
```
plt.figure()
plt.title("Histogram of Color Image Green Channel")
plt.xlabel('Intensity value')
plt.ylabel('pixel count')
plt.stem(hist1)
plt.show()
```
### Histogram Equalization 
```

import cv2
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
```





## Output:
### Input Grayscale Image and Color Image

![Screenshot 2024-03-05 234417](https://github.com/swedha333/Histogram-of-an-images/assets/118720291/4ab90862-ece5-49f3-9cea-b5a52a9f7ecf)

### Histogram of Grayscale Image and any channel of Color Image

![Screenshot 2024-03-05 234430](https://github.com/swedha333/Histogram-of-an-images/assets/118720291/d11369ef-0026-4113-939d-29bac65df179)


### Histogram Equalization of Grayscale Image.

![Screenshot 2024-03-05 234442](https://github.com/swedha333/Histogram-of-an-images/assets/118720291/641fa6fd-90ff-4d1f-8619-89b53eb5207c)



## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
