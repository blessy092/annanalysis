# ANN-diabetes-Progression-Prediction
Artificial Neural Network (ANN) regression project using Scikit-learn's Diabetes dataset to predict disease progression, with data preprocessing, EDA, model training, evaluation, and performance improvement.
# ANN-Based Diabetes Progression Prediction

## Project Overview

This project uses an Artificial Neural Network (ANN) to predict diabetes disease progression using the built-in Diabetes dataset from Scikit-learn.

The objective is to understand how input features relate to a numerical disease progression measure and to develop a regression model using deep learning techniques.

## Objectives

- Load and explore the Diabetes dataset from Scikit-learn.
- Check and handle missing values.
- Normalize input features using StandardScaler.
- Perform Exploratory Data Analysis (EDA).
- Build and train an ANN regression model.
- Evaluate the model using regression metrics.
- Experiment with different ANN architectures and regularization techniques to improve performance.

## Dataset

The project uses the Diabetes dataset available in the Scikit-learn library.

- **Number of samples:** 442
- **Number of input features:** 10
- **Target variable:** A quantitative measure of diabetes disease progression.

The dataset is available directly through Scikit-learn, so no separate dataset download is required.

## Technologies Used

- Python
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- TensorFlow / Keras
- Google Colab or Jupyter Notebook

## Project Workflow

### 1. Data Loading and Preprocessing

- Loaded the Diabetes dataset using `load_diabetes()`.
- Examined dataset dimensions, data types, and summary statistics.
- Checked for missing values and handled them using `SimpleImputer`.
- Split the dataset into training and testing sets.
- Normalized the input features using `StandardScaler`.

### 2. Exploratory Data Analysis

- Visualized feature distributions using histograms.
- Examined correlations using a heatmap.
- Plotted relationships between selected features and the target variable.

### 3. ANN Model Development

- Built a feedforward neural network using Keras.
- Used ReLU activation in the hidden layers.
- Used a linear output layer for regression.
- Compiled the model with the Adam optimizer and Mean Squared Error loss.

### 4. Model Training

- Trained the model using the training dataset.
- Monitored validation loss and Mean Absolute Error.
- Visualized training and validation loss to examine model learning.

### 5. Model Evaluation

The model was evaluated using the following regression metrics:

- Mean Absolute Error (MAE)
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- R² Score

### 6. Model Improvement

Experimented with ANN architecture, L2 regularization, and EarlyStopping to investigate whether the model's generalization performance could be improved.

Compared model performance using consistent evaluation metrics.

## Results

The ANN model achieved an R² score of approximately **0.36** in the reported evaluation.

This indicates that the model explains approximately 36% of the variation in the target values on the evaluated test set.

The result demonstrates that an ANN can be applied to a regression problem, while also highlighting the challenges of training neural networks on small datasets.

*Note: Update this section if your final evaluation produces different results.*

## How to Run the Project

1. Clone this repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Open the project notebook in Google Colab or Jupyter Notebook.

3. Install the required libraries if they are not already installed:

   ```bash
   pip install numpy pandas matplotlib seaborn scikit-learn tensorflow
   ```

4. Run the notebook cells in order, from data loading to model evaluation.

The dataset is loaded directly from Scikit-learn, so no separate dataset file is required.

## Key Learnings

- Data preprocessing and feature scaling.
- Exploratory Data Analysis.
- ANN architecture design using TensorFlow/Keras.
- Regression model training and evaluation.
- Understanding overfitting through training and validation loss.
- Applying regularization and EarlyStopping.
- Comparing model performance using regression metrics.

## Limitations

- The dataset contains only 442 samples.
- The ANN's performance depends on the architecture, training configuration, and data split.
- The model is an educational machine learning project and is not intended for medical diagnosis or clinical decision-making.

## Conclusion

This project provided practical experience in developing an ANN regression model, performing data analysis, evaluating predictions, and experimenting with techniques to improve generalization.

It demonstrates a basic deep learning workflow for a numerical prediction task using Python and TensorFlow/Keras.


