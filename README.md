# EX-09:Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step-1:Initialize an Empty Image:
Create a black image of size 100x600 pixels.
### Step-2:Add Text to the Image:

Use a specified font to write the word "Lifestyle" on the image at a defined position.
### Step-3:Display the Original Image:

Show the image containing the text without axis labels.
### Step-4:Create Structuring Elements:

Define a structuring element for morphological operations (e.g., a cross-shaped kernel).
### Step-5:Erode the Image:

Apply erosion to the image using the defined structuring element to reduce the size of white regions.
### Step-6:Dilate the Image:

Apply dilation to the original image using the same structuring element to increase the size of white regions.

 
## Program:
``` Python
Developed By: P Keerthana
Reference Number: 212223240069
```
# Import the necessary packages
 ```Python
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
# Create the Text using cv2.putText
```python
image = cv2.imread("op.jpg")
```
# Create the structuring element
```python
kernel = cv2.getStructuringElement(cv2.MORPH_RECT, (5, 5))
```
# Plot the original image
```python
plt.figure(figsize=(10, 5))
plt.subplot(1, 3, 1)
plt.imshow(image_rgb)
plt.title("Original Image")
plt.axis("off")
```
### Display the input Image
![image](https://github.com/user-attachments/assets/ffeedde7-bfe7-4ff7-a487-e5b7a8ca4221)
# Erode the image
```python
eroded_image = cv2.erode(image, kernel, iterations=1)
plt.imshow(eroded_image_rgb)
plt.title("Eroded Image")
plt.axis("off")
```
### Display the Eroded Image
![image](https://github.com/user-attachments/assets/408647cd-be5f-4d31-88f8-d7bd545399fe)
<br>
# Dilate the image
```python
dilated_image = cv2.dilate(image, kernel, iterations=1)
plt.imshow(dilated_image_rgb)
plt.title("Dilated Image")
plt.axis("off")
```
### Display the Dilated Image
![image](https://github.com/user-attachments/assets/912f97c5-0eab-4728-9ba2-f92d9a0bcb13)
<br>
## Result:
Thus the generated text image is eroded and dilated using python and OpenCV.
