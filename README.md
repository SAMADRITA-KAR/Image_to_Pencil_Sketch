# Image-to-Pencil-Sketch-Converter

This simple Python program converts an image into a pencil sketch using CV2 library among other tools.

## Description

The conversion process includes changing the picture to grayscale, inverting the image, smoothing the image, and finally converting to a pencil sketch by dividing the grayscale image by the inverse of the smoothened image.

## How to Run the Program

1. Import necessary libraries: CV2, Numpy, Seaborn, and Matplotlib.
2. Load the image and convert it to RGB using CV2.
3. Show the original image using Matplotlib.
4. Convert the original RBG formatted image to grayscale.
5. Invert the grayscale image.
6. Implement the smoothing function on the inverted image.
7. Derive the final sketch by dividing the grayscale image by the inverted smoothed image.
8. Finally, plot the final pencil sketch image.

## Libraries Used

- CV2 to work with images.
- Numpy for numerical operations.
- Seaborn for advanced plotting.
- Matplotlib.pyplot to visualize images in Python.

## Results

The final output is a pencil sketch of the original image. Below are the images to illustrate this:

- Original Image
- Grayscale Image
- Inverted Image
- Smoothened (also Inverted) Image
- Final Pencil Sketch

## Project Files

The project is hosted on a Jupyter Notebook file called "Image to Pencil Sketch.ipynb". The link to the Colab notebook is [here](https://colab.research.google.com/drive/1Oi3g16iKOE6xXEfuyTOoT4giEwGywhYq?usp=drive_link#printMode=true).

## Environment Requirements

Python 3.x and the above-mentioned libraries. The program is currently written to be executed in Google Colab, but it can be run on any Python-supported platform.

## To Execute

Simply upload the "Image to Pencil Sketch.ipynb" in Google Colab and run it.

## Acknowledgements

This project wouldn't have been successful without the help and contribution of the passionate developers in the open-source community. Their hard work and open collaboration inspired me to implement the project and provided me all the resources to get me started.
