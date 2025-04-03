# Histopathologic Cancer Detection

## Overview

This project aims to identify metastatic cancer in small image patches taken from larger digital pathology scans. The goal is to predict the probability that the center 32x32px region of a patch contains at least one pixel of tumor tissue.

## Dataset

The data is a slightly modified version of the PatchCamelyon (PCam) benchmark dataset.

**Dataset Structure:**

* train/ - Contains labeled histopathologic images.
* test/ - Contains unlabeled images for predictions.
* train_labels.csv - A CSV file mapping image IDs to labels (0 = benign, 1 = malignant).

## Approach

1. **Exploratory Data Analysis (EDA):** Analyzed image properties, label distribution, and pixel intensity distribution.
2. **Data Cleaning:** Checked for missing values and duplicates.
3. **Image Preprocessing:**  Utilized `cv2` for loading and converting images to RGB format.
4. **Model Building:** Compared two simple CNN models with varying architectures using Keras Tuner.
5. **Model Evaluation:** Evaluated model performance using accuracy, loss, and ROC-AUC curves.
6. **Prediction and Submission:** Generated predictions on the test set and created a submission file.

## Results

Summarize the key findings and performance metrics of your models here. Include a table or charts to visualize the results.

## Key Findings

Highlight any important observations or insights gained during the project. For example, mention the impact of data augmentation or class weighting on model performance.

## Conclusion

Conclude with a brief summary of the project's outcome and potential future improvements.

## Usage

Provide instructions on how to run the code in a Google Colab environment. Include any necessary dependencies or installation steps.

## Dependencies

List the libraries and packages used in the project:

* TensorFlow
* Keras
* OpenCV (cv2)
* scikit-learn
* Pandas
* NumPy
* Matplotlib
* Seaborn
* PIL (Pillow)
* Keras Tuner
* scikeras

## Acknowledgements

Acknowledge the source of the dataset and any other relevant resources.
