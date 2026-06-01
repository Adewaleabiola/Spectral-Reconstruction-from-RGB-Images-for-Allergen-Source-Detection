**Overview**
This repository contains a deep learning framework for reconstructing hyperspectral images (HSI) from RGB images using the Enhanced Deep Super-Resolution (EDSR) network. The reconstructed spectral information is intended for subsequent allergen source detection in allergen-free food products. The workflow combines image preprocessing, region-of-interest extraction, spectral normalization, deep learning-based spectral reconstruction, and performance evaluation to generate hyperspectral information from conventional RGB images.

**Objectives**
1. Extract regions of interest from hyperspectral and RGB images.
2. Generate paired RGB–HSI datasets for model development.
3. Normalize and preprocess spectral data.
4. Train an EDSR model to reconstruct hyperspectral bands from RGB images.
5. Evaluate reconstruction performance using spectral error metrics.
6. Generate reconstructed hyperspectral datasets for downstream allergen detection and classification tasks.

 **Workflow**
1. Hyperspectral image acquisition and loading.
2. RGB image extraction and preprocessing.
3. ROI segmentation and masking.
4. Dataset preparation and normalization.
5. EDSR model development and training.
6. Spectral reconstruction from RGB images.
7. Model validation and performance assessment.
8. Generation of reconstructed hyperspectral datasets for allergen analysis.

**Model**
The spectral reconstruction framework is based on the Enhanced Deep Super-Resolution (EDSR) architecture implemented in PyTorch.

**Input**
1. RGB images (3 channels)
2. Hyperspectral Images (Multiple spectral Bands)

**Output**
1.  Reconstructed hyperspectral images (multiple spectral bands)
   
**Evaluation Metrics**
The reconstruction performance is assessed using: Mean Relative Absolute Error (MRAE), Root Mean Square Error (RMSE), Visual comparison (Peak Signal-to-noise ratio ) of reconstructed and reference spectra

**Software Requirements**
Python, PyTorch, NumPy, OpenCV, Spectral Python (SPy), Matplotlib, Scikit-image.
**Notes**
This repository focuses on spectral reconstruction from RGB images. The reconstructed hyperspectral data may subsequently be integrated with machine learning models for allergen source detection and food safety applications.
