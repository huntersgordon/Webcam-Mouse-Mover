> for people using python2 and opencv2, please check out the [`lzane:py2_opencv2`](https://github.com/lzane/Fingers-Detection-using-OpenCV-and-Python/tree/py2_opencv2) branch.

## Environment
- OS: MacOS Sierra
- Platform: Python
- Libraries: 
	- OpenCV 3
	- appscript

## How to run?
- run it in python
- press `'b'` to capture the background model (Remember to move your hand out of the blue rectangle)
- press `'r'` to reset the backgroud model

#### Capture background model & Background subtraction
Use background subtraction method called **Gaussian Mixture-based Background/Foreground Segmentation Algorithm** to subtract background. 

For more information about the method, check [Zivkovic2004](http://www.zoranz.net/Publications/zivkovic2004ICPR.pdf)

Here I use the OpenCV's built-in function `BackgroundSubtractorMOG2` to subtract background.

```python
bgModel = cv2.BackgroundSubtractorMOG2(0, bgSubThreshold)
```

# Control-Mouse-With-Hand-OSX
