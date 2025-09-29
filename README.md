This repository contains Exploratory Data Analysis (Part A), Predictive Modelling (Part B), and a Reproducible Workflow Setup (Part C) using Git, Git LFS, and DVC.

Project Structure

├── data/                          # Dataset used in the project
├── models/                        # Saved trained models
│   ├── linear_regression_model.pkl
│   └── logistic_regression_model.pkl
├── iframe_figures/               # Auto-generated figures
├── PartA_EDA.ipynb               # Notebook for Exploratory Data Analysis
├── PartA_EDA.pdf
├── PartB_Modelling.ipynb         # Notebook for Regression and Classification
├── PartB_Modelling.pdf
└── .gitattributes                # Git LFS config

How to Install Dependencies

Prerequisites

Python 3.9 or above

Git and Git LFS – for version control and tracking large files

DVC – for reproducible data and model pipelines

Jupyter Notebook or Visual Studio Code – for running .ipynb notebooks

Apache Spark – required for running Part B’s PySpark models
 
-
Installation

pip install -r requirements.txt

If you don’t have a requirements.txt, install manually:

pip install pandas numpy matplotlib seaborn scikit-learn joblib pyspark dvc

How to Run the Project

1. Clone the Repository

git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

2. Pull Large Files with Git LFS

git lfs pull

3. Open and Run the Notebooks

- PartA_EDA.ipynb: Clean and explore the data
- PartB_Modelling.ipynb: Run regression and classification, save models

What Results to Expect

Linear Regression

- Predicts rating_number using features such as votes and cost
- Two models: 
  - Scikit-learn’s LinearRegression  
  - Custom Gradient Descent implementation  
- Evaluation: Mean Squared Error (MSE)

Logistic Regression

- Classifies restaurants as high/low rating based on threshold
- Evaluation: Accuracy, Confusion Matrix
- Model saved as logistic_regression_model.pkl

Reproducibility (Part C)

- Git LFS used for versioning large files (.csv, .pkl)
- GitHub used for code versioning
- Optionally, DVC can be used to define pipeline stages

To reproduce everything:

dvc repro

Author

Akey-T  
Aiq Tong from University of Canberra
