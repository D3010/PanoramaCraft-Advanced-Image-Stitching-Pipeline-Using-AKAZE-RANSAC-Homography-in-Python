# PanoramaCraft: Advanced Image Stitching Pipeline Using AKAZE, RANSAC & Homography

## 📌 Overview

This repository showcases a comprehensive image stitching pipeline built in Python, combining modern computer vision techniques such as **AKAZE feature detection**, **homography estimation**, and **RANSAC**-based robust transformation estimation. The goal is to generate seamless panoramic images by stitching overlapping photos taken from similar perspectives.

This project is ideal for those interested in **panorama creation**, **computer vision algorithms**, and **image alignment techniques**, and serves as a great foundational project for learning and experimentation.

---

## 🧠 Core Concepts

- **Feature Detection & Description:** Utilizes the AKAZE algorithm to detect and describe keypoints with binary descriptors.
- **Feature Matching:** Matches descriptors between image pairs using squared L2 distance and Lowe's Ratio Test.
- **Homography Estimation:** Computes the transformation matrix using DLT and SVD techniques.
- **RANSAC (Robust Estimation):** Filters out outliers and finds the best-fitting homography matrix.
- **Image Warping & Blending:** Warps images into alignment and blends them into a seamless mosaic.

---

## 🛠️ Technologies Used

- Python 3.x
- OpenCV
- NumPy
- Matplotlib
- Google Colab (optional, used in demo)

---

## 🔍 Pipeline Breakdown

### 1. **AKAZE Feature Detection**
Detects scale-invariant and rotation-invariant keypoints and descriptors using:
```python
cv2.AKAZE_create()

├── Image_Stitching.ipynb      # Jupyter Notebook with full pipeline
├── stitched_result.png        # Output image
├── README.md                  # You're reading it!
├── inputs/
│   ├── img1.jpg
│   └── img2.jpg
└── utils/
    └── homography_utils.py    # Core transformation functions
