# **Finding Lane Lines on the Road — Lane Detection Project**

The goal is to build a computer-vision pipeline capable of detecting lane lines in road images and videos using classic image-processing techniques.

---

## 🚗 **Project Overview**

In this project, you develop a lane-finding algorithm using **Python**, **OpenCV**, and **NumPy**.
The model processes static road images and video frames to identify left and right lane boundaries.

The pipeline includes:

* Color selection / masking
* Grayscale conversion
* Gaussian smoothing
* Canny edge detection
* Defining Region of Interest (ROI)
* Hough Line Transform
* Line extrapolation to draw full-length lane lines

---

## 📁 **Repository Structure**

```
.
├── P1.ipynb                # Main notebook containing the full lane detection pipeline
├── test_images/            # Input sample images
├── test_images_output/     # Output images with detected lanes
├── test_videos/            # Input sample videos
├── test_videos_output/     # Output videos with detected lanes
└── README.md               # Project documentation
```

---

## 🧠 **Pipeline Steps**

### **1. Import Dependencies**

Uses:

* OpenCV (cv2)
* NumPy
* Matplotlib

### **2. Color Selection**

Extracts white/yellow lane markings using thresholding and masks.

### **3. Grayscale Conversion**

Simplifies image → makes edge detection easier.

### **4. Gaussian Blur**

Reduces noise to avoid false edges.

### **5. Canny Edge Detection**

Finds strong lane edges.

### **6. Region of Interest (ROI) Masking**

Keeps only the triangular area where lanes appear.

### **7. Hough Transform**

Detects line segments in the ROI.

### **8. Line Averaging & Extrapolation**

Combines detected segments into clear left & right lane lines.

### **9. Draw Lane Lines**

Overlays the detected lanes on the input image/video.

---

## ▶️ **Running the Project**

### **Requirements**

Install dependencies:

```bash
pip install numpy matplotlib opencv-python
```

### **Run the Notebook**

```bash
jupyter notebook P1.ipynb
```

---

## 🎥 **Output**

The project produces:

* Processed images with lane lines highlighted
* Processed driving videos with continuous lane overlays

---

## 📌 **Key Learnings**

* Classical Computer Vision without Deep Learning
* Working with image masks & ROIs
* Edge detection and Hough Transform
* Video frame-by-frame processing
* Basic autonomous driving perception concepts

---

## 🚀 **Future Improvements**

* Use color space transformations (HLS, HSV) for better detection
* Implement lane curvature estimation
* Add robustness for different lighting/weather conditions
* Upgrade to Deep Learning–based lane detection (CNNs)

---