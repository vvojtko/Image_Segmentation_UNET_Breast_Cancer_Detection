# majorProject
 
Python project made for my major project/dissertation purposes. The program performs binary image segmentation on breast ultrasound images.
As a first step, the program process data with specified image processing technique which resulted in following datasets:
1. Original dataset
2. Blob detection using Laplacian of Gaussian dataset
3. Canny-edge detection dataset
4. Multi-Otsu thresholding preceded by normalization & median filtering dataset
5. Median filter and normalization dataset
6. 3-channel image where for each channel is used different method
 a. Canny-edge detection, Blob detection, Median&Normalization
 b. Canny-edge detection, Original, Blob detection
 c. Canny-edge detection, Multi-Otsu thresholding, Median&Normalization
 d. Median&Normalization, Blob detection, Original

While having different datasets, the UNET model was trained and tested using every single dataset and the results were
compared using dice coefficient. The results could be valuable insights in developing CAD systems for breast cancer detection using BUS images.

Project achieved first grade from both markers (the best grade you can get).

Abstract from the paper:

This paper presents an investigation into the impact of pre-processing on Breast Cancer
Image Segmentation using a deep learning network on Ultrasound images only. In 2020,
breast cancer became the world's most commonly diagnosed cancer, and early detection is
a significant key in fighting that. To detect cancer using computer-aided-detection (CAD)
software, it needs first to perform segmentation as it is a part of the staging process and a
standard step before doing classification. Breast ultrasound (BUS) images are challenging
due to the noise which can make segmentation inaccurate. The project aimed to perform a
series of image pre-processing techniques on the BUS images to minimize noise's negative
effect or enhance the image and use the pre-processed images as input for a deep-learning
network. Different pre-processing methods were applied to the original dataset and used as
input for the deep-learning model (U-Net). The project compares the output of the network
using IoU, Dice-Coefficient measures the impact of many pre-processing techniques to find
the most efficient one among them, for BUS images to achieve the most accurate results of
image segmentation and to highlight the unique characteristic of the BUS data. The analysis
of results could be a valuable insight in developing CAD systems for breast cancer detection
and classification. 
