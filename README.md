Task 04 - Hand Gesture Recognition Model Using CNN

Dataset: https://www.kaggle.com/datasets/gti-upm/leapgestrecog

The Python file task04.py performs all the tasks involved in building a hand gesture recognition model using Convolutional Neural Networks (CNN).

-Project Overview
This project focuses on developing a hand gesture recognition model capable of identifying and classifying various hand gestures from image data. The model can be used to enable intuitive human-computer interaction or gesture-based control systems.

-Key Steps in the Project
1. Data Loading:
The dataset was loaded from the provided Kaggle link using the Kaggle API. It contains images of hand gestures that were classified into 8 categories (e.g., Fist, Five, Point, etc.).

2. Data Augmentation and Preprocessing:
To handle the variability in the dataset, I applied data augmentation techniques, including rescaling, random zoom, shearing, and horizontal flipping. The images were resized to 64x64 pixels and normalized by scaling the pixel values between 0 and 1.

3. Model Architecture:
I constructed a Convolutional Neural Network (CNN) model with the following layers:

Convolution layers (for feature extraction)
MaxPooling layers (for downsampling)
Dropout layers (for regularization)
Fully connected Dense layers (for classification)
4. Model Training:
The model was trained using the training dataset and validated using a validation dataset, both of which were split from the main dataset. The Adam optimizer and categorical cross-entropy loss function were used for training.

5. Evaluation:
The model was evaluated using the validation dataset, and performance metrics such as accuracy were computed. The final model achieved significant accuracy in predicting hand gestures.

6. Saving the Model:
The trained model was saved in HDF5 format (.h5) to allow for reuse in future projects or further fine-tuning.

7. Prediction Functionality:
A function was added to allow users to upload an image of a hand gesture and get the model's prediction. This can be used for testing the model with unseen data.

Class Labels:
The gestures recognized by the model are as follows:

Fist
Five
Point
Swing
Ok
Peace
Rock
Thumb

-Model Performance
The model’s performance was evaluated based on accuracy metrics. The accuracy on the validation set reached X% after 10 epochs of training. You can further improve the performance by fine-tuning the model architecture or using a larger dataset.

-Visualization
A confusion matrix and other relevant performance metrics (such as accuracy and loss) can be plotted to visually evaluate the model's performance.
