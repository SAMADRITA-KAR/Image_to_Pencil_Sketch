# Pencil Sketch Image Transformer

This Python-based project uses OpenCV, NumPy, Seaborn, and Matplotlib to transform regular images into pencil sketches. 

## Table of Contents

1. [Getting Started](#getting-started)
2. [Prerequisites](#prerequisites)
3. [Usage](#usage)
4. [Results](#results)
5. [Contributing](#contributing)
6. [License](#license)

## Getting Started

Clone the repository onto your local machine and install the required dependencies to get a local copy up and running.

## Prerequisites

The following Python packages are needed:

- OpenCV
- NumPy
- Seaborn
- Matplotlib

To install the packages using pip, run:

```bash
 pip install opencv-python numpy seaborn matplotlib 
```
Usage
Load the image and use the following commands to convert it to a pencil sketch:
# Import libraries
import cv2
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

# Load and plot the image
i=cv2.imread("Portrait.jpg")
i=cv2.cvtColor(i,cv2.COLOR_BGR2RGB)

plt.figure(figsize= (6,6))
plt.imshow(i)
plt.axis("off")
plt.title("Original")
plt.show()

# Convert image to grayscale
ig = cv2.cvtColor(i, cv2.COLOR_BGR2GRAY)

plt.figure(figsize= (6,6))
plt.imshow(ig, cmap="gray")
plt.axis("off")
plt.title("Grayscale")
plt.show()

# Invert the image
im = 255 - ig

plt.figure(figsize= (6,6))
plt.imshow(im, cmap="gray")
plt.axis("off")
plt.title("Inverted")
plt.show()

# Smoothen the image
bi = cv2.GaussianBlur(im, (21,21), sigmaX=0, sigmaY=0)

plt.figure(figsize= (6,6))
plt.imshow(bi, cmap="gray")
plt.axis("off")
plt.title("Smoothened")
plt.show()

# Final sketch
f = cv2.divide(ig, 255 - bi, scale=255)

plt.figure(figsize= (6,6))
plt.imshow(f, cmap="gray")
plt.axis("off")
plt.title("Final Sketch")
plt.show()

## Results

The final output is a beautiful pencil sketch of the original image.

## Contributing

For major changes, please open an issue first to discuss what you would like to change. Contributions are always welcome!

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.

Remember to update this README template with your specific paths, names, or other details as necessary.


