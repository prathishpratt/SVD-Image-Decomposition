# Image Compression using Singular Valued Decomposition

### Supervisor:

Dr. Tsui-Wei Weng

### On:

Nov 28, 2023

### Course:

DSC 210 FA’23 Numerical Linear Algebra

---

### Team:

- Dinesh Karthikeyan
PID: A59026248
Halıcıoğlu Data Science Institute
- Nandita Sanjivi
PID: A69027955
Halıcıoğlu Data Science Institute
- Prathish Murugan
PID: A69027919
Halıcıoğlu Data Science Institute

## Introduction

Image Compression is the process of reducing the size of the image without significantly compromising its visual quality. This is essential for various applications, including storage, transmission and efficient utilization of resources. 

In this project, we explore the conventional linear algebra-based approach as well as the state-of-the-art approach for image compression. The comparison of Singular Value Decomposition (SVD) with the SOTA approach of using High Fidelity Generative Compression.

## SVD Approach
Singular Value Decomposition (SVD) serves as a robust mathematical tool for image compression. By decomposing an image matrix into three constituent matrices—U, Σ (Sigma), and V^T—SVD enables a more concise representation of the original image. 

The key to compression lies in selectively retaining the first k singular values and their associated columns in U and V. The truncated singular values are then utilized to reconstruct the compressed image matrix. This process, while introducing some loss, allows for a substantial reduction in data size, making it an efficient method for optimizing storage, transmission, and computational resources.

## State Of The Art Approach
This study extensively explores the integration of Generative Adversarial Networks (GANs) and learned compression techniques to create a state-of-the-art generative lossy compression system. The investigation covers normalization layers, generator and discriminator architectures, training strategies, and perceptual losses. Notably, the outcomes include visually pleasing reconstructions with perceptual similarity to the input, operation across a broad range of bitrates, and applicability to high-resolution images. In bridging the gap between rate-distortion-perception theory and practical implementation, the approach is assessed quantitatively using various perceptual metrics and through a user study.

## Result Comparison - Visual Representation

![image](https://github.com/prathishpratt/SVD-Image-Decomposition/assets/49114256/21286054-d39a-43f0-bc8d-19e445d99eeb)

## Compare and contrast

Compare results from the earlier approach and SOTA implementation.

The visual quality of the images becomes unacceptable when the number of singular values is decreased. Optimizing a neural compression scheme with a GAN yields reconstructions with high perceptual fidelity that are visually close to the input. Users of HiFiC method can benefit from better reconstructions at lower bitrates, reducing the amount of storage needed to save pictures and the bandwidth required to transmit pictures.

![image](https://github.com/prathishpratt/SVD-Image-Decomposition/assets/49114256/e68d779a-aabe-4194-be88-e9ec6e752cc7)

## Conclusion

Image compression using SVD and HiFiC techniques are evaluated based on their performance using perceptual metrics.  Since we are computing the SVD, SSIM and multiplying the U, S and V matrices together on each round of the algorithm, its performance is poor than the generally accepted compression techniques today. In conclusion, the SVD approach proved robust, simple, easy to implement, and efficient in a constrained environment
