# Style Transfer Colab

This project implements Neural Style Transfer (NST) on images and videos using TensorFlow and TensorFlow Hub models in a Google Colab environment. It combines artistic style transfer with super-resolution to create high-quality stylized images and videos with color fidelity and detail preservation.

## Features

- Neural style transfer on images and videos.
- Luminance-based style transfer to preserve original colors.
- High-resolution output using ESRGAN super-resolution.
- Frame-by-frame video style transfer support.
- Easy-to-use interface via Google Colab notebooks.
- Organized input/output management for content, style, and results.

## How the Project Works

This project performs Neural Style Transfer (NST) on images and videos by combining deep learning models with image enhancement techniques to produce visually appealing artistic outputs.

### Workflow Overview

1. **Input**  
   Users provide a **content image** or video and a **style image** (artistic reference). These inputs can be uploaded through the Google Colab interface or placed in designated folders.

2. **Neural Style Transfer**  
   The project uses TensorFlow Hub pre-trained models to compute style transfer. It applies the style primarily on the **luminance channel** to preserve the content’s original colors. For videos, style transfer is applied frame-by-frame.

3. **Super-Resolution Enhancement**  
   After style transfer, the project enhances the output using ESRGAN (Enhanced Super-Resolution Generative Adversarial Network). This step increases the resolution and sharpness of the stylized outputs, generating high-definition images and videos.

4. **Output**  
   Stylized images and videos are saved in organized folders. Outputs retain original content details with added artistic style and improved quality.

### Summary  
The project combines artistic style application with advanced super-resolution techniques to achieve high-quality, color-faithful visual results on both images and videos. It is designed to be user-friendly with modular code, making it easy to run and customize within the Google Colab environment.

## Acknowledgments

- TensorFlow and TensorFlow Hub for models.
- Google Colab for the cloud environment.
- ESRGAN for super-resolution enhancement.
- OpenCV for video and image processing.
- Academic papers and community implementations on neural style transfer and color fidelity algorithms.

