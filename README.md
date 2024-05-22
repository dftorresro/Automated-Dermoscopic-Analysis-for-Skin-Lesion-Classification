# Skin Lesion Classification Challenge

*All the details in the article.*

## Overview
This repository contains all the materials and code for the skin lesion classification project conducted from February 26, 2024, to April 28, 2024. The goal is to classify dermoscopic images of skin lesions into one of eight diagnostic classes using advanced machine learning techniques, with a focus on the ABCD rule of dermoscopy—evaluating Asymmetry, Border irregularity, Color, and Dimension.

## Dataset
The dataset includes 25,331 dermoscopic images of skin lesions, along with available metadata. It is pre-split into a training-validation set (75%) and a test set (25%).

## Methodology

### Feature Extraction
We employ the ResNet model architecture for feature extraction. By removing the final layer, we use the extracted features as input to a Support Vector Machine (SVM) classifier, combining deep learning with traditional machine learning for enhanced classification performance.

### Modified ResNet + SVM Architecture
This approach uses ResNet's deep representational learning capabilities and SVM's robust classification performance, which is particularly effective for the imbalanced nature of our dataset.

## Further Improvements
### Leveraging the ABCD Rule
To further enhance the model's accuracy and sensitivity to subtle dermatological features, future work could focus on more detailed and robust extraction of features based on the ABCD rule:
- **Asymmetry:** Implement algorithms that can quantify asymmetry more precisely in lesion images.
- **Border Irregularity:** Use advanced edge detection techniques to assess and quantify border irregularities more effectively.
- **Color:** Employ color analysis techniques that can detect slight variations in color distribution within a lesion.
- **Dimension:** Integrate more sophisticated methods to measure the size and shape variations across the lesion's area.

These improvements aim to harness deeper insights from dermatological features, potentially leading to better diagnostic accuracy and earlier detection of skin cancers.

## Results
This section will detail the performance of the ResNet + SVM model on the test set, with visualizations or confusion matrices to illustrate the model's effectiveness.
