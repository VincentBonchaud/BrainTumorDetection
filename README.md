# BrainTumorDetection

The goal of this project was to train a deep learning model to predict brain tumors from medical images.

To perform image segmentation and correctly predict the tumor, we chose to use a slightly customized structure of CNN: U-Net.

This model architecure learned the feature mapping of the image and using the same mapping to convert the vector back to the image again. This preserves the structural integrity of the image which reduce distortion enormously.

### Results

We compared result with and without preprocessing on the images.

Without preprocessing:
- Dice coefficient : 0.5059,
- F1 score : 0.6049,
- Recall : 0.5778

With preprocessing:
- Dice coefficient : 0.5305,
- F1 score : 0.5985,
- Recall : 0.5971

The 2D approach is better with preprocessing (0.53 vs 0.50)