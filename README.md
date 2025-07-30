# Penguin Species Classification – Machine Learning Project

## Project Overview

This project explores the use of supervised machine learning models to classify penguin species based on measurable physical traits. Built around the **Palmer Penguins** dataset, this work aims to provide an approachable, interpretable, and effective alternative to the overused Iris dataset.

The notebook and methods draw inspiration from Parul Pandey’s popular Kaggle notebook, “Penguin Dataset — The New Iris,” with additional custom exploration, model testing, and enhancements.

## Dataset Summary

- **Source:** [Kaggle - Penguin Dataset: The New Iris](https://www.kaggle.com/code/parulpandey/penguin-dataset-the-new-iris)
- **Original Data Origin:** Palmer Station LTER and the palmerpenguins R package
- **Observations:** 344 individual penguins
- **Target:** Penguin species (`Adelie`, `Gentoo`, `Chinstrap`)
- **Features:**
  - Island
  - Bill length (mm), bill depth (mm)
  - Flipper length (mm)
  - Body mass (g)
  - Sex
  - Year of observation

## Workflow

1. **Data Loading**
   - Read dataset with pandas, explored initial structure and types.

2. **Data Cleaning**
   - Removed nulls and non-informative values.
   - Encoded categorical data for model compatibility.

3. **Exploratory Data Analysis (EDA)**
   - Distribution plots for all features by species.
   - Correlation matrix and feature importance.
   - Pairplots, boxplots, and group-wise comparisons.

4. **Modeling and Evaluation**
   - Models tested:
     - Logistic Regression
     - K-Nearest Neighbors (KNN)
     - Decision Tree Classifier
     - Random Forest Classifier
   - Metrics:
     - Accuracy
     - Confusion Matrix
     - Classification Report (precision, recall, F1)
   - Cross-validation used where applicable.

5. **Model Selection**
   - The Random Forest Classifier achieved the highest accuracy.
   - Key features included: `flipper_length_mm`, `bill_length_mm`, and `bill_depth_mm`.

## Deliverables

- **Code**: Jupyter Notebook (`Penguin Jupyter.ipynb`) containing all data processing, visualizations, and modeling.
- **Project Report**: This `README.md` file summarizing the approach, results, and how to run the project.
- **Technical Presentation Summary**:
  - Brief overview suitable for technical interviews, including model decisions, feature insights, and classification results.

## Results

- **Best Model**: Random Forest Classifier
- **Accuracy**: ~97%
- **Notable Findings**:
  - `Flipper length` and `bill size` are the most influential features.
  - Adelie penguins were the most common in the dataset.
  - Islands contributed to separation of certain species (e.g., Chinstrap only observed on Dream Island).

## Running the Project

1. Clone this repository:
   ```bash
   git clone https://github.com/sorzit/PENGUINS.git
   cd PENGUINS
