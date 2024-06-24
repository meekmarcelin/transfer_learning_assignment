Fruit and Vegetable Classification using Transfer Learning
Description
This project focuses on applying transfer learning techniques to classify fruits and vegetables. The objective is to leverage pre-trained models and fine-tune them for specific tasks, thereby reducing training time and improving performance.

Dataset
The dataset used for this task is the "fruit-and-vegetable-image-recognition" dataset. It contains images of various fruits and vegetables organized into different classes. Each class represents a specific type of fruit or vegetable, and the task is to classify images into these categories.

Evaluation Metrics
The performance of the fine-tuned models is evaluated using the following metrics:

Accuracy: The proportion of correctly classified samples out of the total number of samples.
Loss: The value of the loss function used during training, indicating how well the model is performing.
Precision: The ratio of true positive predictions to the total number of positive predictions.
Recall: The ratio of true positive predictions to the total number of actual positive samples.
F1 Score: The harmonic mean of precision and recall, providing a balance between the two metrics.
Methodology
Data Preparation:

Configured Kaggle API in Google Colab to download and unzip the "fruit-and-vegetable-image-recognition" dataset.
Prepared training and validation data generators with data augmentation techniques (rotation, shift, and horizontal flip).
Model Setup:

Imported necessary libraries and set parameters for batch size, epochs, and learning rate.
Loaded pre-trained models (VGG16, ResNet50, InceptionV3) with ImageNet weights.
Fine-Tuning:

Added custom top layers (GlobalAveragePooling2D and Dense layers).
Froze the pre-trained layers to retain learned features and trained only the new top layers.
Training and Evaluation:

Trained the models using the training data generator.
Evaluated the models on the validation data generator.
Saved the trained models.
Prediction:

Made predictions using one of the trained models to verify its performance on the validation set, demonstrating successful transfer learning with fine-tuning of the top layers.
