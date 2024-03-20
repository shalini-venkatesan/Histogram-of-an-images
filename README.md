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
# Developed By: 
# Register Number:
```
### Grayscale Image and Color Image
```
import cv2
import matplotlib.pyplot as plt
Gray_image = cv2.imread('dip.jpeg')
Color_image = cv2.imread('p.jpeg')
plt.imshow(Gray_image)
plt.show()
plt.imshow(Color_image)
plt.show()
```
### Histogram
```
plt.figure()
plt.title("Histogram")
plt.xlabel('grayscale value')
plt.ylabel('pixel count')
plt.stem(hist)
plt.show()
```

### Histogram Equalization
```
import cv2
gray_image = cv2.imread("i11.jpg",0)
cv2.imshow('Grey Scale Image',gray_image)
equ = cv2.equalizeHist(gray_image)
cv2.imshow("Equalized Image",equ)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
## Output:
### Input Grayscale Image and Color Image
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/82ee26f7-be6e-486c-9c1f-dee8f21dc324)



![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/4bd8a3c5-a4b2-49de-a4d1-7ddb2e51f583)
### Histogram of Grayscale Image and any channel of Color Image
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/45630f20-e3be-45ec-8bdb-c91017f85bc9)

![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/c4ea87be-8a38-4b3a-93d3-9cf844877833)

### Histogram Equalization of Grayscale Image.

![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/fdc5b9a7-05b4-4985-ba5a-9693224a991f)



## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
