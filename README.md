# Finger Sign Classification using CNN

A deep learning project that classifies hand finger signs (1–5) using a Convolutional Neural Network (CNN). The model is trained on labeled hand gesture images and predicts the corresponding finger count from an input image.

## Features

* Finger sign classification (1–5)
* Image preprocessing and normalization
* CNN-based image classification
* Training and evaluation on labeled datasets
* Model performance visualization
* Supports prediction on new images

## Technologies Used

* Python
* TensorFlow
* Keras
* NumPy
* OpenCV
* Matplotlib

## Model Architecture

* Data Augmentation
* Convolutional Layers
* Max Pooling Layers
* Flatten Layer
* Dense Layers
* Softmax Output Layer

The model is trained on a labeled hand sign dataset where each image corresponds to a finger count between 1 and 5.

## Workflow

1. Load the dataset.
2. Preprocess and normalize images.
3. Train the CNN model.
4. Validate model performance.
5. Evaluate on the test dataset.
6. Predict finger signs for unseen images.

## Project Structure

```text
├── finger_sign_detection.ipynb # Complete training and testing notebook
├── Signs_Data_Training.h5 # Training dataset
├── Signs_Data_Testing.h5 # Testing dataset
├── requirements.txt # Project dependencies
├── README.md
```

## Installation

1. Clone the repository.
2. Install the required dependencies:

   ```
   pip install -r requirements.txt
   ```
3. Train the model:

   ```
   python train.py
   ```
4. Predict on an image:

   ```
   python predict.py
   ```

## Dataset

This project uses the **Signs Detection Dataset** from Kaggle.

Download the dataset automatically using:

```python
import kagglehub

path = kagglehub.dataset_download("maneesh99/signs-detection-dataset")
```

Or download it manually from Kaggle and place the following files in the project directory:

* `Signs_Data_Training.h5`
* `Signs_Data_Testing.h5`


## License

This project is open-source and intended for educational and research purposes.
