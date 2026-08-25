# Handwritten Character Recognition

A Convolutional Neural Network (CNN) based machine learning project for recognizing handwritten digits using the MNIST dataset.

## Project Overview

This project uses a CNN to classify handwritten digits from 0 to 9. The model is trained on the MNIST dataset and evaluated using test accuracy, test loss, and a confusion matrix.

## Dataset

The project uses the MNIST handwritten digit dataset.

- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels
- Number of classes: 10 (digits 0–9)

## Technologies Used

- Python
- TensorFlow / Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

## Model Architecture

The CNN consists of:

- Conv2D layer with 32 filters
- MaxPooling2D
- Conv2D layer with 64 filters
- MaxPooling2D
- Flatten layer
- Dense layer with 128 neurons
- Dropout layer
- Output Dense layer with 10 neurons

## Model Performance

- Test Accuracy: **99.24%**
- Test Loss: **0.0234**

The model also achieved correct predictions on sample handwritten digits and was evaluated using a confusion matrix.

## Project Structure

```text
CodeAlpha_HandwrittenCharacterRecognition/
│
├── data/
│
├── models/
│   └── handwritten_character_cnn.keras
│
├── notebooks/
│   └── Handwritten_Character_Recognition.ipynb
│
├── README.md
└── requirements.txt

## Results

The CNN achieved a test accuracy of **99.24%** on the MNIST test dataset.

A confusion matrix was used to analyze classification performance across all 10 digit classes. The model also successfully predicted sample handwritten digits from the test dataset.

Example:

- Actual digit: 7
- Predicted digit: 7

## How to Run

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Open the notebook:

```text
notebooks/Handwritten_Character_Recognition.ipynb
```

Run the notebook cells from top to bottom.

## Internship

This project was completed as part of the CodeAlpha Machine Learning Internship.
