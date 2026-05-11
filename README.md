 🍎 Fruit Freshness Detection using Deep Learning (VGG16)

 📌 Overview

This project aims to classify fruits based on their **type** and **freshness status** (Fresh or Rotten) using deep learning techniques.

The model is built using a pre-trained
VGGNet
(VGG16) and applies **Transfer Learning** to achieve high accuracy with limited training time.



 🎯 Objectives

Classify fruit images into:

  * Fresh Apples
  * Fresh Banana
  * Fresh Oranges
  * Rotten Apples
  * Rotten Banana
  * Rotten Oranges
Build an efficient image classification model
Apply transfer learning using a pre-trained CNN


🗂️ Dataset

The dataset used in this project is available on Kaggle:

👉 https://www.kaggle.com/datasets/sriramr/fruits-fresh-and-rotten-for-classification

 Dataset Features:

* Contains images of:

  * Apples, Bananas, Oranges
* Each category is labeled as:

  * Fresh
  * Rotten
* Organized into:

  * Training set
  * Test set

---

🛠️ Technologies Used

* Python
* TensorFlow / Keras
* NumPy
* Matplotlib
* ImageDataGenerator

---

 ⚙️ Model Architecture

* Pre-trained **VGG16** (without top layers)
* Input size: **150 × 150 × 3**
* Added layers:

  * AveragePooling2D
  * Flatten
  * Dense (64 neurons, ReLU)
  * Dropout (0.5)
  * Output layer (6 classes, Softmax)

---

🔄 Training Details

* Optimizer: Adam (learning rate = 0.001)
* Loss Function: Categorical Crossentropy
* Batch Size: 15
* Epochs: 5

Data Augmentation:

* Rotation (15°)
* Horizontal Flip

---

📊 Results

Training Accuracy: 82.68%
Validation Accuracy: 91.11%
Test Accuracy: 90.51%
Test Loss: 0.3347

Observations:

* Good performance on clear images
* Minor errors with partially rotten fruits

 🧪 Testing

The model was evaluated using:

* Accuracy
* Validation metrics
* Loss curves
* Random image predictions



 📌 Future Improvements

* Increase number of epochs
* Add more fruit categories
* Apply fine-tuning on VGG16 layers
* Improve dataset diversity

---

👩‍💻 Author

Amany Ismail 

---

⭐ Notes

This project demonstrates how transfer learning can be used effectively for real-world image classification tasks in agriculture and food quality inspection.
