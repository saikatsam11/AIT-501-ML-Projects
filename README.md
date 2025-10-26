# Weight Category Classification - Machine Learning Project

## Project Description
This project implements machine learning models to classify individuals into weight categories based on their lifestyle habits, dietary patterns, and demographic information. The multiclass classification task predicts 7 distinct weight categories ranging from Underweight to severe Obesity levels.

## Dataset Information
- **Records**: 15,533 complete entries
- **Numerical Features**: Age, Height, Weight, BMI, FCVC, NCP, CH2O, FAF, TUE
- **Categorical Features**: Gender, Family History, FAVC, CAEC, SCC, CALC, MTRANS
- **Target Variable**: 7 weight categories (Insufficient Weight, Normal Weight, Overweight I, Overweight II, Obesity I, Obesity II, Obesity III)

## Models Implemented
Three machine learning algorithms were developed and evaluated:

### 1. K-Nearest Neighbors (KNN)
- **Best Parameters**: k=15, distance weights, Manhattan metric
- **Performance**: 86.23% test accuracy

### 2. Random Forest
- **Best Parameters**: 300 trees, max_depth=20, bootstrap=False
- **Performance**: 90.39% test accuracy

### 3. XGBoost (Best Performing)
- **Best Parameters**: 800 estimators, max_depth=3, learning_rate=0.07
- **Performance**: 91.29% test accuracy

## Key Findings
- XGBoost demonstrated superior performance with the highest accuracy
- BMI showed strong correlation with weight classification (0.94 with Weight)
- Lifestyle factors had weaker correlations with obesity levels
- Dataset was well-balanced across target categories

## Project Structure
- `data/` - Dataset files and preprocessing scripts
- `notebooks/` - Exploratory data analysis and experimentation
- `result/` - Best performing model outputs

## Technologies Used
- Python
- Scikit-learn
- XGBoost
- Pandas, NumPy
- Matplotlib, Seaborn
