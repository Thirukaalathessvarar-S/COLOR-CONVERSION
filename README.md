# COLOR-CONVERSION
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Import opencv.

### Step2:
Read the original Image. 

### Step3:
Store the required conversion of the image in a variable.

### Step4:
Show the image stored in the given variable.

### Step5:
Destroy all the windows and end the program. 

## Program:
```python
# Developed By: Thirukaalathessvarar S
# Register Number: 212222230161
```

## i) Convert BGR and RGB to HSV and GRAY
```
import cv2
starry = cv2.imread('gta5.jpg')
cv2.imshow('Original Image', starry)
hsv_image = cv2.cvtColor(starry,cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV',hsv_image)
hsvImage1=cv2.cvtColor(starry,cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV',hsvImage1)
grayImage = cv2.cvtColor(starry,cv2.COLOR_BGR2GRAY)
cv2.imshow('BGR2GRAY',grayImage)
grayImage1 = cv2.cvtColor(starry,cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY',grayImage1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```



## ii)Convert HSV to RGB and BGR
```
import cv2
hsv_image2 = cv2.imread('gta5.jpg')
cv2.imshow('Original HSV Image',hsv_image2)
RGBImage = cv2.cvtColor(hsv_image2,cv2.COLOR_HSV2RGB)
cv2.imshow('BGR2HSV',RGBImage)
BGRImage = cv2.cvtColor(hsv_image2,cv2.COLOR_HSV2BGR)
cv2.imshow('RGB2HSV',BGRImage)
cv2.waitKey(0)
cv2.destroyAllWindows()
```


## iii)Convert RGB and BGR to YCrCb
```
import cv2
boom = cv2.imread('gta5.jpeg')
cv2.imshow('Original HSV Image',boom)
YCrCb_image = cv2.cvtColor(boom, cv2.COLOR_RGB2YCrCb)
cv2.imshow('BGR2HSV',YCrCb_image)
YCrCb_image1 = cv2.cvtColor(boom, cv2.COLOR_BGR2YCrCb)
cv2.imshow('RGB2HSV',YCrCb_image1)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

# iv)Split and Merge RGB Image
```
import cv2
image = cv2.imread('gta5.jpg')
blue = image[:,:,0]
green = image[:,:,1]
red = image[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)
mergeBgr = cv2.merge((blue,green,red))
cv2.imshow('Merged BGR image',mergeBgr)
cv2.waitKey(0)
cv2.destroyAllWindows()
```

#3 v) Split and merge HSV Image
```
import cv2
image = cv2.imread('gta5.jpg')
hsv = cv2.cvtColor(image,cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue - Image',h)
cv2.imshow('Saturation - Image',s)
cv2.imshow('Gray - Image',v)
mergedHSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',mergedHSV)
cv2.waitKey(0)
cv2.destroyAllWindows()
```
## Output:
### i) BGR and RGB to HSV and GRAY
![dip1_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/f55db0aa-f30b-4445-a7a2-ad17710f461f)


![dip2_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/6b288bfc-c8d6-4972-81b4-27bda80caa69)


![dip3_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/e18699b1-5bd9-450f-a09d-48706ca453f7)

![dip4_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/6feb2d28-2d59-4271-8c49-1197075e44d4)

![dip5_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/4ea033ab-c2f6-407a-b9df-d17b0b77ee26)

### ii) HSV to RGB and BGR

![dip_exp333](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/5dc11ded-ea3c-482f-ad0c-e7a88a2ac44e)

![dip6_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/51ad0eba-c5e7-49d4-9cb7-82135c463255)

![dip7_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/e9c44fe7-b184-4539-b990-3310ee51015b)

### iii) RGB and BGR to YCrCb

![dip_exp333](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/6ffdf0c9-a9e9-4b80-9039-1a2730e6111e)

![dip8_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/203875fe-0858-47af-8901-bfd5437692ef)

![dip9_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/f49909a9-83f6-413f-a06e-c89cc61fcc4f)

### iv) Split and merge RGB Image

![dip13_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/765d9733-6bfe-4644-afa3-a2ae43aeb533)

![dip12_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/4245a61c-56da-465d-818f-3d96f20e7d18)

![dip11_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/21e01862-a844-4170-91b1-a3b1afdd3376)

![dip10_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/a818f51d-594d-4490-b199-b31be38be622)

### v) Split and merge HSV Image

![dip14_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/ffbfe722-fbe4-4901-957f-cef8ffd62d6f)

![dip15_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/f387133e-51a4-40f9-9691-29a7926f83bb)

![dip16_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/52ed7672-ea76-4015-af68-6d470be78bc8)

![dip17_exp3](https://github.com/Thirukaalathessvarar-S/COLOR-CONVERSION/assets/121166390/d8f2d440-6e16-4a2b-91cb-37a857fb0597)

## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
