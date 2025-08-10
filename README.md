Neural Style Transfer for Images and Videos
This project implements Neural Style Transfer (NST) on images and videos using TensorFlow and TensorFlow Hub models. It allows you to apply the artistic style of one image onto another content image or video, producing high-quality stylized outputs. The project also includes an HD enhancement step with super-resolution and color-preserving techniques to keep the stylized outputs visually true to the inspiration style.

Features
Neural style transfer on both images and videos.

High-definition (HD) output images with super-resolution enhancement.

Color preservation by applying style transfer primarily on luminance while retaining original color fidelity.

Interactive upload prompts for content image, style image, and optional video in Google Colab.

Frame-by-frame video processing with balanced HD resolution for efficient and clear outputs.

Easy-to-use, modular Python code leveraging TensorFlow Hub models.

Output saving in organized folders with downloadable image and video stylized results.

Getting Started
Prerequisites
Python 3.x

TensorFlow 2.x

TensorFlow Hub

OpenCV

Pillow

Jupyter Notebook or Google Colab environment (recommended for ease of use)

Installation
You can install the required Python packages using:

bash
pip install tensorflow tensorflow-hub opencv-python pillow matplotlib
Usage
Clone the repository or download the project files to your local machine or Google Colab.

Open the notebook or Python script in Colab or your local environment.

Run the code, and when prompted, upload:

Content image: the image you want to stylize.

Style image: the artistic style reference.

Optional input video: for video style transfer.

The program will process the inputs, apply neural style transfer, enhance images to HD quality with super-resolution, preserve colors better, and save results in the sample_outputs/ directory:

Stylized HD image: stylized_image_hd_desat.jpg

Stylized video (if uploaded): stylized_video.mp4

Download and view your stylized images and videos.

Key Functions and Pipeline
load_img(): Loads and scales input images to HD resolution.

stylize_image(): Applies style transfer on images.

super_resolve_image(): Enhances stylized images using ESRGAN super-resolution.

reduce_saturation(): Controls oversaturation to keep colors faithful to the style image.

process_video(): Processes input video frame-by-frame to produce stylized video output.

Interactive upload prompts in Google Colab to simplify user experience.

Results
The project generates visually appealing stylized images and videos that retain fine details and color fidelity while applying the artistic style, enabled by careful luminance-based style transfer and high-resolution super-resolution.

Future Enhancements
Apply super-resolution on video frames for HD video output.

Add adjustable style strength and saturation controls in the UI.

Implement user-friendly web demo using Gradio or interactive notebook widgets.

Explore advanced color transfer methods for further color fidelity improvements.

Acknowledgments
TensorFlow Hub models by Google Magenta for neural style transfer and ESRGAN super-resolution.

TensorFlow and OpenCV libraries for deep learning and image/video processing.

Inspiration from academic papers on neural style transfer and color preservation techniques.
