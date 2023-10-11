# Computational-Photography

This repo is for the coursework of Computer Vision and Computational Photography at UC Berkeley.

## [Project 1: Images of the Russian Empire: Colorizing the Prokudin-Gorskii Photo Collection](https://inst.eecs.berkeley.edu/~cs180/fa23/upload/files/proj1/kai.ma/CS%20180%20Project%201%2092b9fadaefee4f3aa91afcb31b633aa9.html)


1. **Single-Scale Method:** This method involves comparing two images by measuring the Sum of Squared Differences (SSD) for each possible shift for the central 80% windows. The goal is to find the shift that results in the minimum SSD, indicating the best alignment of the two images.
   
2. **Multi-Scale Method:** This method uses an image pyramid to enhance the efficiency and accuracy of alignment. Instead of searching for the best shift at the original resolution, the images are downscaled, and the best shift is identified at this lower resolution. This rough alignment at a coarser scale guides the search at higher resolutions. Once the best shift at the lower resolution is identified, the method scales up the shift and refines the search at the original scale.




---

## [Project 2: Fun with Filters and Frequencies](https://inst.eecs.berkeley.edu/~cs180/fa23/upload/files/proj2/kai.ma/submission/CS%20180%20Project%202%20fe92eb35c05d4421abbab90b21f2987e.html)


- **Finite Difference Operator:** Utilizes convolution to compute the image's partial derivatives, highlighting significant intensity changes in the image.
  
- **Derivative of Gaussian (DoG) Filter:** Involves blurring the image with a Gaussian filter and subsequently detecting edges. The DoG method further refines this process, enhancing edge detection.

- **Image "Sharpening":** A technique that enhances the details of an image by emphasizing the differences between the original and its blurred version.
  
- **Hybrid Images:** A method that combines two images, where one provides the low-frequency components and the other provides the high-frequency components, resulting in an image that has characteristics of both.
  
- **Gaussian and Laplacian Stacks:** Techniques that decompose an image into different frequency components, allowing for detailed analysis and manipulation at various scales.
  
- **Multiresolution Blending:** A method that blends images using their Laplacian stacks, ensuring a smooth transition and integration of details from both images.
