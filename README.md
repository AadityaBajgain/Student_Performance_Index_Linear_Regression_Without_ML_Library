# Student Performance Prediction (Scratch ML)

This project explores a student performance dataset and implements a multivariate
linear regression model from scratch (using NumPy) to predict the
`Performance Index` based on study habits and activity features.

## Project contents
- `student_performance_using_scratch_ml_algorithm.ipynb`: End-to-end notebook
  with data loading, EDA, preprocessing, model training, and evaluation.
- `Student_Performance.csv`: Dataset with 10,000 student records.

## Features used
The model uses the following inputs:
- Hours Studied
- Previous Scores
- Sleep Hours
- Sample Question Papers Practiced
- ECA (binary encoding of `Extracurricular Activities`, Yes=1, No=0)

Target:
- Performance Index

## Notebook workflow
1. Load the dataset and inspect basic stats.
2. Convert `Extracurricular Activities` to a numeric `ECA` feature and drop the
   original column.
3. Split data into train/test using a fixed random seed (80/20).
4. Normalize features using mean and standard deviation from the training set.
5. Train a linear regression model with gradient descent.
6. Evaluate with mean squared error (MSE) on train and test sets.
7. Run sample predictions.

## Requirements
- Python 3.x
- NumPy
- Pandas
- Seaborn
- Jupyter Notebook

Install dependencies (example):
```bash
pip install numpy pandas seaborn jupyter
```

## How to run
```
bash
jupyter notebook student_performance_using_scratch_ml_algorithm.ipynb
```

## Notes
This is a learning-focused implementation that avoids scikit-learn to show the
math and training loop directly in NumPy.
