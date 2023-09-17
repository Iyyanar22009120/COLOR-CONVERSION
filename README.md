# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
## Step1:
import cv2 library and upload the image or capture an image.

## Step2:
Read the saved image using cv2.imread("filename.jpg").

## Step3:
Convert the image into the given color transformation using cv2.cvtColor(image, cv2.BGR2YCrCb) and similarly for other color formats.

## Step4:
Split and merge the image using cv2.split(hsv) and cv2.merge([h,s,v]).

## Step5:
Output the image using cv2.imshow("OUTPUT", image).
## Program:
```python
# Developed By:IYYANAR S
# Register Number:212222240036
# i) Convert BGR and RGB to HSV and GRAY
```
# i) Convert BGR and RGB to HSV and GRAY
```python
import cv2
houseImage = cv2.imread('dip.jpg')
cv2.imshow('212222240036_IYYANAR ,houseImage)
hsvImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsvImage)
hsvImage1=cv2.cvtColor(houseImage,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(houseImage,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(houseImage,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```




# ii)Convert HSV to RGB and BGR

```
import cv2
houseHSVImage = cv2.imread('dip.jpg')
cv2.imshow('212222240036_IYYANAR',houseHSVImage)
RGBImage = cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage=cv2.cvtColor(houseHSVImage,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# iii)Convert RGB and BGR to YCrCb
```
import cv2
houseImage = cv2.imread('dip.jpg')
cv2.imshow('212222240036_IYYANAR',houseImage)
YCrCb_image = cv2.cvtColor(houseImage, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(houseImage, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



# iv)Split and Merge RGB Image

```
import cv2
image = cv2.imread('dip.jpg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('212222240036_IYYANAR',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```


# v) Split and merge HSV Image
```
import cv2
image = cv2.imread('dip.jpg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('212222240036_IYYANAR',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindow()



```
## Output:
### i) BGR and RGB to HSV and GRAY
![1DI](https://github.com/Iyyanar22009120/COLOR-CONVERSION/assets/118680259/111f51f9-02a5-4132-ba45-d9d0eec9f6ad)


### ii) HSV to RGB and BGR
![2DI](https://github.com/Iyyanar22009120/COLOR-CONVERSION/assets/118680259/4f3c23ed-a857-445c-aa2b-c84eff9a18de)


### iii) RGB and BGR to YCrCb
![3DI](https://github.com/Iyyanar22009120/COLOR-CONVERSION/assets/118680259/ae6bd35b-4e3e-40f6-b318-595ee5ec0090)


### iv) Split and merge RGB Image
![4DI](https://github.com/Iyyanar22009120/COLOR-CONVERSION/assets/118680259/113923f8-8d52-4b65-8bf5-d16d93f3be86)


### v) Split and merge HSV Image
![5DI](https://github.com/Iyyanar22009120/COLOR-CONVERSION/assets/118680259/018e37ee-1f85-4d0e-824d-ece4c88516c0)


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
