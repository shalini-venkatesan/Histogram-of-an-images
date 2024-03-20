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
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/a4251306-be99-41e0-af29-29fb1f21357f)




![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/3a871848-bdb4-4c8d-b2a4-995cc0fb1ba5)
### Histogram of Grayscale Image and any channel of Color Image
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/01631636-bc07-4937-a404-3e1abbf17fb0)

### Histogram Equalization of Grayscale Image.
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/8797ed86-76f7-432c-a7ec-a92d33665c1f)




## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
