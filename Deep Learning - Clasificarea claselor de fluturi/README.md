📌 Project Description

The project focuses on classifying butterfly images using both traditional machine learning methods and convolutional neural networks (CNNs), including a model built from scratch and a pre-trained model (MobileNetV2).

📂 Dataset Split

The dataset was divided into 80% for training, 10% for validation, and 10% for testing, using stratification to maintain class proportions. Data loading and augmentation were performed using ImageDataGenerator.

⚙️ Data Preprocessing

Images were resized to standard dimensions (180x180 or 224x224 pixels). Augmentation techniques such as rotations, zoom, and horizontal flipping were applied. For MobileNetV2, the model-specific preprocessing function was also used.

🤖 Methods Used

🔹 CNN from scratch – network with convolutional, pooling, normalization, and dense layers.

🔹 Random Forest – trained on feature vectors extracted from images.

🔹 Pre-trained CNN (MobileNetV2) – used as a feature extractor and fine-tuned.

📊 Results

Model performance on the test set was as follows:

🔹 Simple CNN – 73% accuracy

🔹 Random Forest – 31% accuracy

🔹 Pre-trained CNN (MobileNetV2) – 88% accuracy

The MobileNetV2 model achieved the best results, confirming the effectiveness of transfer learning in image classification.
