# Image-Deskewer
This repository provides a simple Python solution for automatically correcting the skew of images using OpenCV. 

## **Overview**
The script performs the following steps:
1. Converts the input image to grayscale.
2. Applies Gaussian blur for noise reduction.
3. Uses thresholding to create a binary image.
4. Merges text into lines using morphological operations.
5. Finds the largest text block using contours.
6. Computes the skew angle using a minimum area bounding box.
7. Rotates the image to deskew it.

## **Functions**
- `getSkewAngle(cvImage)`: Computes the skew angle of the input image.
- `rotateImage(cvImage, angle)`: Rotates the image around its center.
- `deskew(cvImage)`: Detects the skew angle and corrects it.
