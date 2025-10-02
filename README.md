# Image PCA Analysis with Eigen-Decomposition

This repository demonstrates **Principal Component Analysis (PCA)** on RGB images to derive **Eigenfaces** (or Eigenimages) using **channel-wise PCA**. Unlike traditional PCA on grayscale images, this notebook applies PCA separately to the Red, Green, and Blue channels and then combines them for visualization and reconstruction.

## Repository Structure

```

image-pca-analysis/
│
├─ data/    # Place your RGB images here (jpg/png)
│
├─ eigenfaces_rgb_images.ipynb   # Main notebook
└─ README.md

````

## Notebook Overview

**Notebook:** `eigenfaces_rgb_images.ipynb`

### Sections

1. **Setup and Configuration**
   - Imports required libraries (`numpy`, `PIL`, `matplotlib`, `sklearn.decomposition.PCA`).
   - Sets parameters like image size, number of components, and number of eigenfaces to visualize.

2. **Data Loading and Preprocessing**
   - Loads and resizes images.
   - Separates RGB channels and flattens each channel into feature vectors.

3. **Channel-wise PCA and Eigenface Calculation**
   - Performs PCA independently for Red, Green, and Blue channels.
   - Computes eigenvectors and mean vectors for each channel.

4. **Explained Variance Analysis**
   - Plots cumulative explained variance per channel.
   - Shows how much information is captured by the top components.

5. **Visualization of Color Eigenfaces**
   - Reshapes and normalizes principal components.
   - Combines RGB channel components to create color Eigenfaces.
   - Displays top N Eigenfaces.

6. **Image Reconstruction**
   - Demonstrates image compression and reconstruction using top principal components.
   - Compares reconstructed images with the original images.

## Requirements

- Python 3.x  
- NumPy  
- Pillow (PIL)  
- Matplotlib  
- Scikit-learn  


## Usage

1. Clone the repository:

2. Add your RGB images to the `data/images/` folder.

3. Open the notebook in Jupyter:

4. Run all cells to perform PCA, visualize eigenfaces, and reconstruct images.
