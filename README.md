## Low-Light Image Enhancement Using CNN
## Project Overview
This project aims to improve the quality of images taken in low-light conditions by leveraging Convolutional Neural Networks (CNNs). Low-light images often suffer from high noise levels, poor visibility, and lack of detail, which can hinder various computer vision tasks. Our objective is to create a CNN-based model that effectively denoises and enhances these images, improving their usability and overall quality.

## Model Architecture
The architecture of our CNN model includes several convolutional layers designed for feature extraction and noise reduction:
- **Input Layer**: Accepts RGB images of any resolution.
- **Convolution Layers**: Multiple layers with 32 filters each, using 3x3 kernels and ReLU activation.
- **Skip Connections**: Added to help retain and utilize information from previous layers.
- **Output Layer**: A convolutional layer with activation to create the final enhanced image.
- Detailed architecture is provided in report pdf.

## PEvaluation Metric
The model's performance is evaluated using the Peak Signal-to-Noise Ratio (PSNR). The final average PSNR on the test dataset is 23.802893.

## How to Run
1. **Clone the Repository**:
    ```sh
   https://github.com/Aimank009/VLG_DenoisingImages.git
    ```
2. **Go to project directory**:
    ```sh
    cd VLG_DenoisingImages
    ```
3. **Run the Main Script**:
    ```sh
    python main.py
    ```
#### Testing Instructions
Place the low-light images you want to enhance in the test/low folder. After running the script, the denoised images will be saved in the test/predicted folder.

A sample low-light image is included in the test/low folder, with its corresponding denoised output in the test/predicted folder. To test with your own images, replace the sample image with your own low-light images.
