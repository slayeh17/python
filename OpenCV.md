## OpenCV in Python

### 1. Insert and view images using OpenCV

Here is a little code to insert and view an image:
```Python
import cv2 as cv
img=cv.imread("jet.jpg")
cv.imshow("JET",img)
cv.waitKey(0)
```
Here ```import cv2 as cv``` is used to import OpenCV with ```cv``` as the alias. The ```cv.imread()``` function is used to read an image an store it in a variable named ```img```.

Next the ```cv.imshow()``` function is used to show the image with two arguments:
1. Name of the window the image will be diaplayed.
2. Name of the variable(pixel matrix) the image is stored in.

```Python
cv.waitKey(0)
```
tell the program to show the image untill ```0``` is entered otherwise the image window will show and disappear instantly. Inside ```cv.waitKey()``` any desired key can be stated. 

### 2. Resize an image using OpenCV

To resize an image all we need to do is use ```cv.resize()``` function. Where ```cv``` is an alias of ```cv2``` check the above code.

In this function we need to pass the pixel matrix that is the variable where the image is stored, and also pass the resolution as tuples ```()```.

Here is an example: ```cv.resize(img,(1280,720))```.
