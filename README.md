## Summary of Findings

- The baseline Scikit-learn MLPClassifier achieved moderate accuracy, demonstrating the limitations of simple neural networks on image data.
- The simple CNN (TensorFlow/Keras) significantly improved accuracy, showing the effectiveness of convolutional layers for image classification.
- The advanced CNN, with data augmentation and regularization (dropout, early stopping), achieved the highest test accuracy and best generalization, reducing overfitting.
- Data augmentation (random rotations, shifts, zoom) helped the model learn more robust features from limited data.
- Visualizations (confusion matrix, sample predictions) provided insight into model strengths and common misclassifications.

# FashionMNIST_ImageClassification

This project demonstrates image classification on the FashionMNIST dataset using both traditional machine learning and advanced deep learning techniques. It includes:

- **Baseline MLPClassifier**: A simple neural network using Scikit-learn for quick benchmarking.
- **Advanced CNN**: A high-accuracy Convolutional Neural Network built with TensorFlow/Keras, featuring data augmentation, dropout, and early stopping for improved generalization.

## Workflow
1. **Data Download**: Automatically downloads the FashionMNIST dataset using `kagglehub`.
2. **Preprocessing**: Loads data into pandas DataFrames, separates features/labels, and normalizes pixel values.
3. **Model Training**:
	- Trains a baseline MLPClassifier (Scikit-learn).
	- Trains a simple CNN, then an improved CNN with data augmentation and regularization (TensorFlow/Keras).
4. **Evaluation**: Reports accuracy and displays confusion matrix and sample predictions.

## Usage
1. Open the `FashionMNIST_Scikit_90.ipynb` notebook in Jupyter or VS Code.
2. Run all cells in order. Required packages will be installed automatically.
3. Review the results and visualizations at the end of the notebook.

## Requirements
- Python 3.8+
- Jupyter Notebook or VS Code
- Packages: scikit-learn, matplotlib, seaborn, tensorflow, kagglehub, pandas, numpy

## Notes
- The advanced CNN section uses data augmentation and early stopping to maximize test accuracy and prevent overfitting.
- All code is commented for clarity and easy modification.