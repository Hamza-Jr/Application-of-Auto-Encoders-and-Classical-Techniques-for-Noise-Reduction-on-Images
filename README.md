# Application of Autoencoders and Classical Techniques for Image Denoising

## 📌 Objective
The objective of this project is to understand the functioning of autoencoders, implement them, and use them for image denoising. 

This project applies Autoencoders to remove noise from images and compares their performance with classical denoising techniques. Using the MNIST dataset, synthetic noise is added, and denoising methods like Gaussian filtering and median filtering are tested. The performance of each method is evaluated using PSNR and SSIM metrics.

### 1. Data Loading and Preparation
- Load the MNIST dataset and add noise.

### 2. Apply Traditional Filtering Techniques

#### 2.1 Visualization of Classical Filtering Results
![img1 Image](./images/img1.png)

#### 2.2 Quantitative Evaluation of Filtering
**Interpretation of PSNR results:**

- **Mean Filter (12.28):** Provides basic noise reduction but significantly blurs edges, impacting reconstruction quality.
- **Gaussian Filter (12.43):** Slightly better than the mean filter due to Gaussian weighting, which preserves details better.
- **Median Filter (14.20):** Yields the best results by effectively removing impulse noise while preserving sharp edges, improving fidelity to the original images.

### 3. Build an Autoencoder Model

#### 3.1 Autoencoder Construction

##### 3.1.1 Visualization of Results
![img2 Image](./images/img2.png)

##### 3.1.2 Quantitative PSNR Evaluation
**Interpretation of PSNR results:**
Average PSNR: 20.18

#### 3.2 Advanced Autoencoder Model N1
(Adding additional layers)

##### 3.2.1 Visualization of Results
![img3 Image](./images/img3.png)

##### 3.2.2 Quantitative PSNR Evaluation
**Interpretation of PSNR results:**

#### 3.3 Advanced Autoencoder Model N2
(Adding additional layers)

##### 3.3.1 Visualization of Results
![img4 Image](./images/img4.png)

##### 3.3.2 Quantitative PSNR Evaluation
**Interpretation of PSNR results:**
Average PSNR: 19.94

### 4. Comparison of the Three Models' Results
- Comparing the performance of autoencoders for noise reduction.
- ![img5 Image](./images/img5.png)

---
📌 **Note:** The output images and evaluation results are available in the `images/` folder. Make sure to run the notebook to generate the results.
