# MelanomaDetectionAssignment
# Melanoma Detection using CNN

## Problem Statement
To build a CNN-based model that can accurately detect melanoma, a type of cancer that can be deadly if not detected early. Melanoma accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.

## Dataset
The dataset contains 2357 images of 9 different types of skin cancer. The dataset is divided into train and test subdirectories, each containing 9 sub-directories corresponding to the 9 skin cancer types.

## Approach
1. Import necessary libraries and mount Google Drive to access the dataset (if needed).
2. Define paths for train and test datasets.
3. Load the images using `tf.keras.preprocessing.image_dataset_from_directory`.
4. Visualize sample images from each class.
5. Preprocess the data (caching, shuffling, and prefetching).
6. Build a CNN model with convolutional, pooling, and dense layers.
7. Normalize pixel values using `layers.experimental.preprocessing.Rescaling`.
8. Compile the model with appropriate optimizer and loss function.
9. Train the model using the preprocessed datasets.
10. Evaluate the model's performance on the validation set.
11. Visualize training and validation accuracy/loss curves.
12. Analyze the results and identify potential overfitting or underfitting issues.
13. Implement data augmentation techniques (if needed) to mitigate overfitting or underfitting.
14. Retrain the model with augmented data.
15. Evaluate the performance of the retrained model.
16. Analyze class imbalance in the dataset.
17. Use the Augmentor library to balance the classes by adding more samples.
18. Retrain the model with the class-balanced dataset.
19. Evaluate the performance of the final model.

## Usage
1. Clone the repository.
2. Mount your Google Drive to access the dataset (if needed).
3. Update the paths to the train and test datasets.
4. Run the Jupyter Notebook or Python script.

## Results
The initial model achieved an accuracy of around 75-80% on the validation set, with evidence of overfitting. After implementing data augmentation and class rebalancing techniques, the final model's performance improved, and overfitting/underfitting issues were mitigated.

## Future Work
- Explore transfer learning techniques using pre-trained models.
- Experiment with different data augmentation strategies.
- Collect more diverse and balanced data to further improve model performance.

## References
- [Dataset Source]
- [Related Research Papers]
- [Augmentor Library](https://augmentor.readthedocs.io/en/master/)
