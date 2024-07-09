# Transfer-Learning
This repository demonstrates three approaches to using the VGG16 model for transfer learning:

1. Transfer Learning and Feature Extraction with Data Augmentation
2. Transfer Learning with Fine-Tuning
3. Transfer Learning and Feature Extraction without Data Augmentation

## Prerequisites
1. Python 3.x
2. TensorFlow 2.x
3. Keras
4. NumPy
5. Matplotlib
6. scikit-learn
7. Jupyter Notebook (optional but recommended)

## Data Preparation
The data directory should contain three subdirectories: train, validation, and test, each with corresponding images organized in class-specific subdirectories.

### 1. Transfer Learning and Feature Extraction with Data Augmentation
  This approach involves using a pre-trained VGG16 model to extract features from images while applying data augmentation to increase the variety of training data.

#### Steps
1. Load the VGG16 model with pre-trained weights, excluding the top layers.
2. Add new fully connected layers suitable for the new task.
3. Use data augmentation techniques such as rotation, zoom, and horizontal flip.
4. Train the model using the augmented data.

### 2. Transfer Learning with Fine-Tuning
This approach involves unfreezing the last few layers of the pre-trained VGG16 model and training them along with the new fully connected layers to fine-tune the model.

#### Steps
1. Load the VGG16 model with pre-trained weights, excluding the top layers.
2. Add new fully connected layers suitable for the new task.
3. Freeze the initial layers and unfreeze the last few layers of the VGG16 model.
4. Train the model.

### 3. Transfer Learning and Feature Extraction without Data Augmentation
This approach involves using a pre-trained VGG16 model to extract features from images without applying any data augmentation techniques.

#### Steps
1. Load the VGG16 model with pre-trained weights, excluding the top layers.
2. Add new fully connected layers suitable for the new task.
3. Train the model using the original data without augmentation.

## Results
Each approach has its own advantages and can be chosen based on the specific requirements of the task and the available data.
