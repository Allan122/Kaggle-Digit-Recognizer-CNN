# Handwritten Digit Recognition using a Convolutional Neural Network

## Project Overview
This project is a solution for the Kaggle "Digit Recognizer" competition. The goal is to correctly identify handwritten digits (0-9) from a dataset of tens of thousands of images. A Convolutional Neural Network (CNN) was built using TensorFlow and Keras to achieve this.

---

## Dataset
The data is from the classic MNIST database.
* **Training Set:** 42,000 images
* **Test Set:** 28,000 images
* **Image Size:** 28x28 pixels, grayscale

You can find the competition data here: [Kaggle Digit Recognizer](https://www.kaggle.com/competitions/digit-recognizer)

---

## Methodology
1.  **Preprocessing:** The image pixel values were normalized to a range of [0, 1]. The labels were one-hot encoded.
2.  **Model Architecture:** A CNN was constructed with the following layers:
    * Conv2D (32 filters) -> MaxPooling2D
    * Conv2D (64 filters) -> MaxPooling2D
    * Flatten
    * Dense (128 units) with Dropout (0.5)
    * Dense (10 units, softmax output)
3.  **Training:** The model was trained for 15 epochs using the Adam optimizer.

---

## Results
The model achieved a final score of **0.98917** on the Kaggle public leaderboard, successfully classifying over 98.9% of the test images.

* **Validation Accuracy:** ~99.1%
* **Public Leaderboard Score:** 0.98917

You can view my final submission and the complete code in my Kaggle notebook: **https://www.kaggle.com/code/allan143/notebook8f74fc9d5e**

---
