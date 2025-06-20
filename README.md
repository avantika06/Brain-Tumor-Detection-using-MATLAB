# Brain-Tumor-Detection
This project implements an automated brain tumor detection pipeline using MATLAB. The pipeline leverages image segmentation techniques to preprocess MRI images, detect and segment potential tumor regions, and categorize the tumors as 'Benign' or 'Malignant' based on their size.

## Features
Preprocesses MRI images by resizing, converting to grayscale, and binarizing.
Applies Sobel filters for edge detection and watershed segmentation for tumor region identification.
Utilizes morphological operations to refine tumor regions.
Categorizes tumors as 'Benign' or 'Malignant' based on size.
Demonstrates strong problem-solving and medical image processing skills.

## Steps
1. Load and Preprocess Image
* Load MRI image and resize to [200, 200].
* Convert the RGB image to grayscale.
* Convert the grayscale image to a binary image.

2. Edge Detection
* Apply Sobel filter in both horizontal and vertical directions.
* Compute the gradient magnitude for edge detection.

3. Watershed Segmentation
* Perform watershed segmentation on the gradient magnitude image.
* Display the segmented image.

4. Morphological Operations
* Use morphological operations to open and reconstruct the binary image.
* Identify and refine potential tumor regions.

5. Tumor Size Measurement
* Measure the size of the tumor regions in pixels.
* Convert the size from pixels to square centimeters.

6. Tumor Categorization
* Categorize the tumor as 'No tumor', 'Benign', or 'Malignant' based on the calculated size.

## Usage
1. Ensure you have MATLAB installed.
2. Clone this repository:
```bash
git clone https://github.com/avantika06/Brain-Tumor-Detection.git
```
3. Place the MRI image (3.png) in the project directory.
4. Run the MATLAB script `Brain_Tumor.m`
   
## Output
The script will display the following:

* Original MRI image.
* Grayscale image.
* Binarized image.
* Watershed segmented image.
* Image with identified and refined tumor regions.
* Tumor size in square centimeters.
* Tumor category ('No tumor', 'Benign', or 'Malignant').
