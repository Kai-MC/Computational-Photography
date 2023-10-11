# Computational-Photography

This repo is for the coursework of Computer Vision and Computational Photography at UC Berkeley.

## [Project 1: Images of the Russian Empire: Colorizing the Prokudin-Gorskii Photo Collection](https://inst.eecs.berkeley.edu/~cs180/fa23/upload/files/proj1/kai.ma/CS%20180%20Project%201%2092b9fadaefee4f3aa91afcb31b633aa9.html)


1. **Single-Scale Method:** This method involves comparing two images by measuring the Sum of Squared Differences (SSD) for each possible shift for the central 80% windows. The goal is to find the shift that results in the minimum SSD, indicating the best alignment of the two images.
   
2. **Multi-Scale Method:** This method uses an image pyramid to enhance the efficiency and accuracy of alignment. Instead of searching for the best shift at the original resolution, the images are downscaled, and the best shift is identified at this lower resolution. This rough alignment at a coarser scale guides the search at higher resolutions. Once the best shift at the lower resolution is identified, the method scales up the shift and refines the search at the original scale.




---

## [Project 2: Fun with Filters and Frequencies](https://inst.eecs.berkeley.edu/~cs180/fa23/upload/files/proj2/kai.ma/submission/CS%20180%20Project%202%20fe92eb35c05d4421abbab90b21f2987e.html)


- **1.1 Finite Difference Operator:** The image's partial derivatives in the x and y directions are computed using convolution. The gradient magnitude, which represents intensity change, is then calculated. A threshold of 0.18 produces a binary image highlighting the edges.
  
- **1.2 Derivative of Gaussian (DoG) Filter:** The image is first blurred using a 2D Gaussian filter. After blurring, edges are detected with a threshold of 0.08. The Derivative of Gaussians (DoG) method is then applied.

- **2.1 Image "Sharpening":** An image is loaded and its pixel values are normalized. Details are extracted by subtracting a blurred version from the original. By adding back twice the amount of these details to the original, a sharpened effect is achieved. This results in enhanced details, more noise, and increased contrast.
  
- **2.2 Hybrid Images:** Images are converted to grayscale. A function creates hybrid images by applying a low-pass filter to one image and subtracting a low-pass filtered version from another image to get its high-pass version. The frequency components of an image are visualized using Fast Fourier Transform.
  
- **2.3 Gaussian and Laplacian Stacks:** Laplacian stacks are constructed from each image using their corresponding Gaussian stacks. The sigma of the gaussian is selected as 4.
  
- **2.4 Multiresolution Blending:** This involves blending images using Laplacian Stacks.
