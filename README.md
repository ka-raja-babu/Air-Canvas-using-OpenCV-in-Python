# Air-Canvas-using-OpenCV-in-Python
Computer vision project implemented with OpenCV

Ever wanted to draw your imagination by just waiving your finger in air. In this project, an Air Canvas has been built which can draw anything on it by just capturing the motion of a coloured marker with camera. Here a coloured object at tip of a pen is used as the marker.

The computer vision techniques of OpenCV are used here to build this project. The preferred language is python due to its exhaustive libraries and easy to use syntax but by understanding the basics, it can be implemented in any OpenCV supported language.

Here, Colour Detection and tracking is used in order to achieve the objective. The colour marker in detected and a mask is produced. It includes the further steps of morphological operations on the mask produced which are Erosion and Dilation. Erosion reduces the impurities present in the mask and dilation further restores the eroded main mask.

# Algorithm

1)Start reading the frames and convert the captured frames to HSV colour space.(Easy for colour detection)

2)Prepare the canvas frame and put the respective ink buttons on it. 

3)Adjust the trackbar values for finding the mask of coloured marker.

4)Pre-process the mask with morphological operations.(Erosion and dilation).

5)Detect the contours, find the centre coordinates of largest contour and keep storing them in the array for successive frames .(Arrays for drawing points on canvas).

6)Finally draw the points stored in array on the frames and canvas .

# Outputs

![alt text](https://github.com/ka-raja-babu/Air-Canvas-using-OpenCV-in-Python/blob/main/Output%201.png)
![alt text](https://github.com/ka-raja-babu/Air-Canvas-using-OpenCV-in-Python/blob/main/Output%202.png)
![alt text](https://github.com/ka-raja-babu/Air-Canvas-using-OpenCV-in-Python/blob/main/Output%203.png)
![alt text](https://github.com/ka-raja-babu/Air-Canvas-using-OpenCV-in-Python/blob/main/Output%204.png)
