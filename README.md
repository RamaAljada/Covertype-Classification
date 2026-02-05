# Forest Cover Type Classification - Covertype Classification
This project aims to **classify forest cover types** into 7 categories using classic Machine Learning algorithms such as:  
- Decision Tree  
- k-NN  
- SVM  
- Logistic Regression  

## Dataset Description
The project uses the **Covertype Dataset**, a well-known dataset in the ML community for testing classification algorithms on environmental data such as:  
- Elevation  
- Slope of the land  
- Soil type  
- Distances to natural features or infrastructure  

**Main goal:** Predict the last column `Cover_Type`, which represents the forest cover type for each data row.  

### Dataset Notes
- Number of rows: 581,012  
- Number of columns: 55  
- All columns are numeric  
- Some columns were already One-Hot Encoded  
- The dataset is clean, with no missing values  

## How to Get the Dataset
You can download the dataset from **Kaggle** via the official dataset page:  
[Forest Cover Type Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/forest-cover-type-dataset)  

> Note: A Kaggle account is required to download the dataset. Place the downloaded file in your project folder before running the code.

## Project Workflow
1. **Baseline Models:**  
   - Train ML models like Decision Tree, Logistic Regression, SVM, and k-NN.  
   - Use a sample subset if the dataset is too large to speed up training.

2. **Hyperparameter Tuning:**
   - GridSearchCV → Accurate but slow on large datasets.
   - RandomizedSearchCV → Fast, gives near-optimal results, and suitable for large datasets.

3. **Final Evaluation:**  
   - Use **Confusion Matrix** to check the performance of each model on each class.  
   - Compare models using Accuracy and F1-weighted Score.  
   - In this project, the best performance was achieved by the Decision Tree with ~93.9% accuracy.
   
**License: MIT**
