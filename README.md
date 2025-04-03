# 🔍 Computer Vision Feature Detection & Matching  

## 📌 Project Overview  
This project implements three important **feature detection and matching algorithms** using **OpenCV** in Python:  

1. **SIFT (Scale-Invariant Feature Transform)** – Detects and matches key points between two images.  
2. **RANSAC (Random Sample Consensus)** – Filters out incorrect keypoint matches and estimates a transformation.  
3. **Harris Corner Detector** – Identifies and visualizes corner points in an image.  

All implementations are provided in the `B4_59_TA2.ipynb`.  

---

## 📂 Project Structure  

📁 cv_feature_detection
│── 📜 README.md # Project Documentation
│── 📜 B4_59_TA2.ipynb # Python implementation of SIFT, RANSAC, and Harris Corner
│── 🖼️ image1.png # Sample image for feature detection
│── 🖼️ image2.png # Sample image for feature detection
│── 🖼️ image3.png # Sample image for feature detection
│── 📜 requirements.txt # Required dependencies

---

## ⚙️ Installation & Setup  

To run this project, install the required dependencies using:  

pip install -r requirements.txt

Alternatively, install OpenCV and Matplotlib manually:

pip install opencv-python numpy matplotlib
🖼️ Feature Detection & Matching Implementations
1️⃣ SIFT Feature Matching
The SIFT (Scale-Invariant Feature Transform) algorithm detects key points and matches them between two images.
It is scale-invariant and rotation-invariant, making it ideal for object recognition.

Input: Two images

Output: Matched key points between images

Usage: Detects common points in different views of the same object

2️⃣ RANSAC for Outlier Removal & Transformation Estimation
The RANSAC (Random Sample Consensus) algorithm is used to estimate a transformation model while removing incorrect keypoint matches.
It ensures that only reliable feature matches are used for alignment.

Input: Matched keypoints from SIFT

Output: A refined transformation matrix with inlier matches

Usage: Helps in panorama stitching, object tracking, and 3D reconstruction

3️⃣ Harris Corner Detector
The Harris Corner Detector is used to find strong corner points in an image.
Corners are detected based on variations in intensity in different directions.

Input: A single grayscale image

Output: A visualization with red dots marking corners

Usage: Used in motion detection and image registration

🎯 How to Use
Run the SIFT Feature Matching algorithm:

sift_feature_matching("image1.png", "image2.png")
Run the RANSAC Outlier Removal algorithm:

ransac_outlier_removal("image1.png", "image2.png")
Run the Harris Corner Detector:

harris_corner_detection("image1.png")

------------------

🛠️ Dependencies
Python 3.x

OpenCV (opencv-python)

NumPy

Matplotlib

To install the required dependencies:

pip install opencv-python numpy matplotlib

-----------------------

👨‍💻 Author
Uttkarsh Khanke
Created as part of a Computer Vision project implementing feature detection algorithms.