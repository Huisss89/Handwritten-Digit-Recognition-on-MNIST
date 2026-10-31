# Handwritten Digit Recognition on MNIST using k-NN
A machine learning project that explores handwritten digit recognition using the MNIST dataset, with K-Nearest Neighbors (KNN) as the primary classification model. The project also compares its performance against Logistic Regression and Support Vector Machine (SVM) to evaluate the effectiveness of traditional machine learning algorithms.

**Run the project**: https://colab.research.google.com/drive/1WOAckETuqfDMhyPBFa3o_eV3ldc1411g?usp=sharing

## Dataset
The project uses the **MNIST handwritten digit dataset**, which contains 70,000 grayscale images of handwritten digits (0–9), divided into 60,000 training images and 10,000 testing images.

The notebook uses `tf.keras.datasets.mnist.load_data()` to download and load the dataset automatically.

## Objectives
- Preprocess and analyze the MNIST dataset to ensure data quality.
- Implement and optimize KNN, Logistic Regression, and SVM classifiers.
- Compare model performance using multiple evaluation metrics.
- Analyze classification errors, model behavior, and generalization capabilities.

## Technologies Used
- **Python:** Model implementation and data processing
- **TensorFlow:** Loading the MNIST dataset
- **NumPy:** Numerical operations and data manipulation
- **Scikit-learn:** Machine learning models, hyperparameter tuning, and evaluation
- **Matplotlib:** Data visualization and plotting
- **Seaborn:** Statistical data visualization

## Setup and Installation
1. Clone the repository:
   ```bash
   git clone <https://github.com/Huisss89/Handwritten-Digit-Recognition-on-MNIST-using-k-NN->
   cd <https://github.com/Huisss89/Handwritten-Digit-Recognition-on-MNIST-using-k-NN->
   ```
2. Create and activate a virtual environment:
   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```
3. Install the required dependencies:
   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn tensorflow jupyter
   ```
4. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```
5. Open `SourceCode.ipynb` and run all cells.

## Project Workflow

### 1. Data Preprocessing
- Load the MNIST dataset using TensorFlow.
- Verify image dimensions (28 × 28), pixel ranges, and missing values.
- Normalize pixel values from 0–255 to 0–1.
- Flatten images into 784-dimensional feature vectors.
- Convert image data into appropriate numerical data types.
- Check for and remove duplicate records.

### 2. Algorithm Implementation
- **K-Nearest Neighbors (KNN):** Classifies handwritten digits based on the majority class among their nearest neighbors.
- **Logistic Regression:** Predicts digit classes using probability-based classification.
- **Support Vector Machine (SVM):** Classifies digits by identifying decision boundaries that separate different classes.

### 3. Hyperparameter Tuning
Apply **GridSearchCV** to identify suitable model parameters and optimize classification performance.

### 4. Model Evaluation
Evaluate model performance using the following metrics and techniques:

**Evaluation Metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- ROC curves and Area Under the Curve (AUC)
- Matthews Correlation Coefficient (MCC)

**Validation and Analysis:**
- Stratified cross-validation
- Learning curves
- Confusion matrices
- Classification error analysis

### 5. Results and Model Comparison
- **KNN:** Achieved the best overall performance, with **97.14% test accuracy** and the highest F1-score.
- **SVM:** Achieved **94.72% test accuracy**, demonstrating competitive classification performance.
- **Logistic Regression:** Achieved **92.59% test accuracy**, providing a relatively efficient classification approach.

### 6. Visualizations and Analysis
The project includes visualizations to examine model performance and classification behavior, including confusion matrices, learning curves, ROC curves, and examples of correctly and incorrectly classified digits.

### 7. Conclusion
The project demonstrates that traditional machine learning algorithms remain effective for handwritten digit recognition. KNN achieved the highest overall classification performance among the three models, while SVM and Logistic Regression offered alternative approaches with different efficiency and generalization trade-offs.

This project provided practical experience in data preprocessing, machine learning implementation, hyperparameter optimization, model evaluation, and comparative performance analysis.
