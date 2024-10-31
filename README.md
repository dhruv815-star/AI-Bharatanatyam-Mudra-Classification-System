# AI-Based Bharatanatyam Mudra Classification System
Bharatanatyam is one of the oldest classical dance forms of India, renowned for its expressive hand gestures called mudras. These mudras play a crucial role in communicating narratives, emotions, and spiritual concepts in Bharatanatyam performances. However, manually identifying and classifying these intricate hand gestures can be challenging and time-consuming. Therefore, there is a need for automated classification systems to aid practitioners and enthusiasts in understanding and preserving this cultural heritage.

The project aims to automate the identification and classification of Bharatanatyam mudras using Convolutional Neural Networks (CNNs). By leveraging modern deep learning techniques, particularly the Adam optimizer, the system seeks to provide a valuable tool for dancers, instructors, and enthusiasts to enhance their understanding and appreciation of this ancient Indian classical dance form.

## Data Set Description: 
The dataset used for training the CNN model comprises a diverse collection of images depicting various Bharatanatyam mudras. It has been sourced from [Kaggle](https://www.kaggle.com/datasets/sadhanaparameswaran/mudras) and covers a wide range of hand gestures performed within the context of Bharatanatyam dance. The images have been standardized to adhere to a common size (180x180 pixels) and format (RGB color) to ensure consistency and compatibility across the dataset.

## Implementation Methodology
The implementation methodology follows a systematic workflow:
1. **`Data Preprocessing`**: Images are resized, converted to RGB color format, and augmented using techniques such as rotation, flipping, and scaling to increase variability. Pixel values are normalized to [0, 1] to facilitate convergence during training.

2. **`Model Architecture Design`**: A custom CNN architecture comprising three convolutional layers with increasing numbers of filters (16, 32, and 64), followed by max-pooling layers and a fully connected layer, is utilized. Rectified Linear Unit (ReLU) is used as the activation function to introduce non-linearity.

3. **`Model Training`**: The dataset is split into 80% training data and 20% testing data. Data augmentation is applied to the training data to prevent overfitting. The Adam optimizer is employed to adaptively adjust the learning rate during training, accelerating convergence and enhancing stability.

4. **`Model Evaluation`**: The model is evaluated on metrics such as accuracy, validation accuracy, etc., to assess its performance in classifying Bharatanatyam mudras.

The detailed diagram highlighting the CNN architecture used and the flow is depicted in fig.[1](model_flow.png) and fig.[2](model_architecture.png) respectively.

## Results and Discussion
The CNN model trained with the Adam optimizer demonstrates promising results in classifying Bharatanatyam mudras accurately. Compared to models trained without optimization, the optimized model exhibits faster convergence, higher accuracy, and improved stability during training. The use of Adam optimizer significantly enhances the efficiency and effectiveness of the model, leading to better classification performance.

## Future Scope
Future research and development avenues include exploring alternative optimizers, fine-tuning hyperparameters, refining the CNN architecture, and expanding the dataset to improve classification accuracy further. Additionally, the system could be extended to recognize and classify other aspects of Bharatanatyam performances, such as facial expressions and body postures.


