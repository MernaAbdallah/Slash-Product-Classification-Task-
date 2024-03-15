## Product Classification using Convolutional Neural Networks (CNNs)

![image](https://github.com/MernaAbdallah/Slash-Product-Classification-Task-/assets/91502893/8e1758c0-2df7-4f5c-a72b-14862b041058)

### Overview
In this project, I aim to classify products into different categories using Convolutional Neural Networks (CNNs). The dataset was collected from the Slash application and consists of various product images across different categories. I divided the dataset into training and testing sets and performed preprocessing to prepare the images for model training.

### Preprocessing Steps
1. **Resizing**: All images are resized to a specified target size (150, 150) to ensure uniform dimensions for model training.
   
2. **Normalization**: Pixel values of the images are rescaled to the range [0, 1] using the `rescale=1 / 255` parameter in the `ImageDataGenerator`. This normalization stabilizes the training process and improves convergence.

3. **Data Augmentation**: Various techniques such as rotation, width and height shifting, zooming, and horizontal flipping are applied to augment the training data. This increases the diversity of the training set and improves the model's robustness.

### Model Development and Evaluation
I implemented several CNN architectures and evaluated their performance on the test dataset. Additionally, techniques such as regularization and early stopping were applied to prevent overfitting and improve model accuracy.

#### Models Implemented:
1. **Model 1**: A simple CNN architecture with convolutional and pooling layers followed by dense layers. Achieved test accuracy: 67.61%.

2. **Model 2**: A more complex CNN architecture with additional convolutional and pooling layers. Achieved test accuracy: 45.17%.

3. **Model 3**: A deep CNN architecture with further complexity. Achieved test accuracy: 18.18%.

### Observations
- Model performance varied based on the complexity of the architecture.
- More complex models tended to overfit on the small dataset, leading to reduced performance on the test set.
- Simple models achieved better generalization and higher test accuracy.

### Conclusion
When dealing with a small dataset, it's essential to strike a balance between model complexity and generalization. Simple models often perform better and are less prone to overfitting. Regularization techniques and early stopping can further improve model performance.

This repository contains the code for preprocessing, model development, training, evaluation, and optimization, providing insights into building a robust product classification system using deep learning techniques.
