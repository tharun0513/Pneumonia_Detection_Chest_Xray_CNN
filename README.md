# Pneumonia Detection from Chest X-ray Images Using Deep Learning

## Project Overview

This project was developed as part of a Machine Learning course to classify chest X-ray images as either Normal or Pneumonia using deep learning techniques. The project compares the performance of a Custom Convolutional Neural Network (CNN) with a pre-trained MobileNetV2 model using transfer learning.

The main objective is to determine which model provides better accuracy and overall performance for pneumonia detection from chest X-ray images.

---

## Dataset

The project uses the Chest X-Ray Images (Pneumonia) dataset available on Kaggle.

The dataset consists of chest X-ray images divided into two classes:

- Normal
- Pneumonia

The images are already separated into training, validation, and testing folders.

---

## Project Workflow

The project follows these steps:

1. Import the required Python libraries.
2. Load the chest X-ray dataset.
3. Preprocess the images by resizing and normalizing them.
4. Apply data augmentation to improve model generalization.
5. Build and train a Custom CNN model.
6. Build and train a MobileNetV2 transfer learning model.
7. Evaluate both models using different performance metrics.
8. Compare the results and determine the better-performing model.

---

## Models Used

### Custom CNN

The custom CNN was built using multiple convolutional and max-pooling layers followed by batch normalization, dropout, and fully connected layers.

### MobileNetV2

MobileNetV2 is a pre-trained deep learning model that uses transfer learning. The final classification layers were replaced with custom layers to perform binary classification on chest X-ray images.

---

## Data Preprocessing

The following preprocessing techniques were applied:

- Resize images to 224 × 224
- Normalize pixel values
- Data augmentation including:
  - Rotation
  - Zoom
  - Horizontal flipping
  - Width shift
  - Height shift

These techniques help improve the model's ability to generalize to unseen data.

---

## Performance Evaluation

Both models were evaluated using:

- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- Classification Report

According to the experimental results, MobileNetV2 achieved better overall performance than the Custom CNN, showing the effectiveness of transfer learning for this classification task.

---

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Pandas
- Matplotlib
- Scikit-learn

---

## Repository Structure

```
├── Pneumonia_Detection.ipynb
├── README.md
├── main.tex
├── Bibliography.bib
├── Final_Report.pdf
├── Figures/
└── models/
```

---

## Running the Project

1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repository.git
```

2. Install the required libraries:

```bash
pip install tensorflow keras numpy pandas matplotlib scikit-learn
```

3. Open the notebook in Jupyter Notebook or upload it to Kaggle and run all the cells.

---

## Results

The project demonstrates that transfer learning can improve the performance of medical image classification tasks. MobileNetV2 produced higher accuracy than the Custom CNN and showed better overall classification performance on the test dataset.

---

## Future Improvements

Some possible improvements for future work include:

- Training on a larger and more diverse dataset.
- Testing additional transfer learning models such as EfficientNet or DenseNet.
- Implementing explainable AI techniques such as Grad-CAM to visualize model predictions.
- Performing hyperparameter optimization to further improve performance.

---

## Author

Gajula Tharun Kumar

Machine Learning Course Project

---

## Acknowledgements

- Kaggle for providing the Chest X-ray Pneumonia dataset.
- TensorFlow and Keras for the deep learning framework used in this project.
