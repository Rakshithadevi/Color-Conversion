# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:

# Step1: Import cv2 and save and image as filename.jpg
# Step2: Use imread(filename, flags) to read the file
# Step3: Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.
# Step4: Split and merge the image using cv2.split and cv2.merge commands.
# Step5: End the program and close the output image windows.

## Program:
```
# Developed By:RAKSHITHA DEVI J
# Register Number:212221230082
```
```
### i) Original image
import cv2
uni = cv2.imread('uni.jpg')
cv2.imshow('Original image',uni)
cv2.waitKey(0)
cv2. destroyAllWindows()

### ii) Convert BGR to HSV 
import cv2
uni = cv2.imread('uni.jpg')
hsv_image = cv2.cvtColor(uni, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV' ,hsv_image )
cv2.waitKey(0)
cv2. destroyAllWindows()

### iii) Convert BGR to GRAY
import cv2
uni = cv2.imread('uni.jpg')
gray_image = cv2.cvtColor(uni, cv2.COLOR_BGR2GRAY)
cv2.imshow( 'BGR2GRAY', gray_image)
cv2.waitKey(0)
cv2. destroyAllWindows()

### iV) Convert RGB to HSV
import cv2
uni = cv2.imread('uni.jpg')
hsv_image = cv2.cvtColor(uni, cv2.COLOR_RGB2HSV)
cv2.imshow('RGB2HSV', hsv_image)
cv2.waitKey(0)
cv2. destroyAllWindows()

### V) Convert RGB to GRAY
import cv2
uni = cv2.imread('uni.jpg')
gray_image1 = cv2.cvtColor (uni, cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()

### Vi) Convert HSV to RGB
import cv2
uni = cv2.imread('uni.jpg')
RGB_image = cv2.cvtColor(uni,cv2.COLOR_HSV2RGB)
cv2.imshow('HSV to RGB',RGB_image )
cv2.waitKey(0)
cv2.destroyAllWindows()

### vii) Convert HSV to BGR
import cv2
uni = cv2.imread('uni.jpg')
BGR_image = cv2.cvtColor(uni,cv2.COLOR_HSV2BGR)
cv2.imshow('HSV to BGR',BGR_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

### viii) Convert RGB to YCrCb
import cv2
uni = cv2.imread('uni.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

### ix) Convert BGR to YCrCb
import cv2
uni = cv2.imread('uni.jpg')
YCrCb_image = cv2.cvtColor(uni, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb',YCrCb_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

### x) Split RGB Image
import cv2
uni = cv2.imread('uni.jpg')
blue=uni[:,:,0]
green=uni[:,:,1]
red=uni[:,:,2]
cv2.imshow('B-Channel',blue)
cv2.imshow('G-Channel',green)
cv2.imshow('R-Channel',red)

### xi) Merge RGB Image
merged_BGR=cv2.merge((blue,green,red))
cv2.imshow('Merged BGR Image',merged_BGR)
cv2.waitKey(0)
cv2.destoryAllWindows()

### xii) Split HSV Image
import cv2
uni = cv2.imread('uni.jpg')
hsv=cv2.cvtColor(uni,cv2.COLOR_BGR2HSV)
h,s,v=cv2.split(hsv)
cv2.imshow("Hue-image",h)
cv2.imshow("Saturation-image",s)
cv2.imshow("gray-image",v)

### xiii) Merge HSV Image
Merged_HSV=cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()


```
## Output:
### i) Original image

![image](https://user-images.githubusercontent.com/94165326/227579701-17eb3e1c-70dc-4bf1-88ce-d20f2093282d.png)


### ii) Convert BGR to HSV 

![image](https://user-images.githubusercontent.com/94165326/227580129-e120cb22-79da-4fec-a0ef-455cdfc168b9.png)


### iii) Convert BGR to GRAY

![image](https://user-images.githubusercontent.com/94165326/227580361-b99e17b6-ce42-4ee1-9b7b-dc73ac34a096.png)



### iV) Convert RGB to HSV

![image](https://user-images.githubusercontent.com/94165326/227580648-a575270a-f121-4b8f-b2f8-c79f280e72f7.png)



### V) Convert RGB to GRAY

![image](https://user-images.githubusercontent.com/94165326/227580848-f0dd4088-7fd4-4266-a1b5-42b008e1328f.png)


### Vi) Convert HSV to RGB

![image](https://user-images.githubusercontent.com/94165326/227581157-3ac29c81-ee82-4bac-bff0-ecf63e86049c.png)



### vii) Convert HSV to BGR

![image](https://user-images.githubusercontent.com/94165326/227581424-081bb50d-db6e-47a8-b6e5-df15ad5bdf36.png)


### viii) Convert RGB to YCrCb

![image](https://user-images.githubusercontent.com/94165326/227581656-807a87dc-702e-4f31-8685-13a726ee9eb5.png)



### ix) Convert BGR to YCrCb

![image](https://user-images.githubusercontent.com/94165326/227581900-b36d672d-6565-4333-85ea-0641acf7a4d0.png)



### x) Split RGB Image
![image](https://user-images.githubusercontent.com/94165326/227584652-ff6ab2c3-a8dd-4095-bd46-af06ec47d8ff.png)



### xi) Merge RGB Image

![image](https://user-images.githubusercontent.com/94165326/227585080-08fa15f7-e0e2-4b2c-b8b9-0d35ac7b3e38.png)



### xii) Split HSV Image

![image](https://user-images.githubusercontent.com/94165326/227585746-7525d4a5-1fe6-491c-9e21-0a5f19400d2e.png)



### xiii) Merge HSV Image

![image](https://user-images.githubusercontent.com/94165326/227585876-a11f2128-adc1-415a-abce-cb23c0ebb613.png)



## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
