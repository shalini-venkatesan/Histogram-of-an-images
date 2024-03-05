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

```
## Output:
### Input Grayscale Image and Color Image
![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/35ea401a-c4fb-4967-8584-aa4f0484e764)


### Histogram of Grayscale Image and any channel of Color Image

![image](https://github.com/shalini-venkatesan/Histogram-of-an-images/assets/118720291/909ab7f6-1d94-4229-a736-69a98f3bf176)


### Histogram Equalization of Grayscale Image.




## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
