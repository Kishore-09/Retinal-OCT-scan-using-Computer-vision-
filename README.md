# Retinal OCT Scan Classification using Computer Vision

This project uses a Kaggle dataset of Optical Coherence Tomography (OCT) scans to analyze and classify retinal images. The project implements **Canny Edge Detection** and **Gaussian Blurring** techniques to verify and preprocess the scans. Various machine learning classifiers were explored for potential classification tasks.

---

## Dataset
The dataset contains OCT scans of four retinal conditions:
- **CNV** (Choroidal Neovascularization)
- **DME** (Diabetic Macular Edema)
- **DRUSEN**
- **NORMAL**

Dataset source: [Kaggle OCT Dataset 2017](https://www.kaggle.com/paultimothymooney/kermany2018)

- **Training Data**: Images from `/train` directory.
- **Testing Data**: Images from `/test` directory.

---

## Project Workflow
### 1. **Data Preprocessing**
- Read and load images from the dataset.
- Applied **Gaussian Blurring** to reduce noise.
- Resized images to a uniform size of **224x224 pixels** for consistency.

### 2. **Visualization**
- Displayed original scans alongside their processed (edge-detected) counterparts.
- Plotted the distribution of training data across the four classes using a pie chart.

### 3. **Edge Detection**
- Implemented **Canny Edge Detection** to highlight boundaries within the scans.
- Visualized edge-detected scans for each condition to verify features.

### 4. **Machine Learning Classifiers**
Explored multiple classifiers for potential classification tasks:
- **Random Forest**
- **AdaBoost**
- **Gradient Boosting**
- **K-Nearest Neighbors**
- **Support Vector Machines**
- **Naive Bayes**
- **Logistic Regression**

---

## Key Code Features
- **Data Exploration**: Loaded images and visualized their distribution.
- **Image Processing**: Applied transformations like Gaussian blur and edge detection.
- **Visualization**: Displayed processed images to validate results.
- **Pie Chart**: Highlighted the class distribution in the training dataset.

---

## Libraries Used
- **Core Libraries**: `numpy`, `pandas`, `math`, `os`
- **Visualization**: `matplotlib`, `seaborn`
- **Image Processing**: `cv2` (OpenCV)
- **Machine Learning**: `sklearn` (for various classifiers and metrics)

---

## Results
1. **Visualization of Preprocessing**:
   - Original scans alongside edge-detected scans for all four classes were successfully visualized.
   - Gaussian blur effectively smoothed the images, enhancing the results of edge detection.

2. **Dataset Class Distribution**:
   - Pie chart analysis showed a balanced or imbalanced class distribution, aiding in understanding dataset biases.

---

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/Kishore-09/Retinal-OCT-scan-using-Computer-vision-.git
