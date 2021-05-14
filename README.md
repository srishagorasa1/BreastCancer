# BreastCancer Detection

**Introduction** 
Breast cancer is a malignant cell growth in the breast. If left untreated, the cancer spreads to other areas of the body. Excluding skin cancer, breast cancer is the most common type of cancer in women in the United States, accounting for one of every three cancer diagnoses. Breast cancer ranks second among cancer deaths in women.

**Problem statement**
The goal of this project is the application of several data mining and machine learning techniques to classify whether the tumor mass is benign or malignant. This will help in understanding the important underlaying importance of attributes thereby helping in predicting the stage of breast cancer depending on the values of these attributes. Through the understanding of nature of attributes in cancer prediction, the healthcare community can perform additional research corresponding to these attributes to help prevent pervasion of breast cancer.

**Exploratory data analysis**
The EDA process will help in understanding the nature of the dataset and help in identification of potential outliers or correlated variables.


**Project description:**
This project consists of using a CNN neural net model to predict (classification) breast cancer detection on the public dataset of breast cancer available in the package datasets of scikitlearn.
The dataset contains information of 569 women across 32 different attributes. 1) ID number 2) Diagnosis (M = malignant, B = benign)

Ten real-valued features are computed for each cell nucleus:
1. radius (mean of distances from center to points on the perimeter)
2. texture (standard deviation of gray-scale values)
3. perimeter
4. area
5. smoothness (local variation in radius lengths)
6. compactness (perimeter^2 / area - 1.0)
7. concavity (severity of concave portions of the contour)
8. concave points (number of concave portions of the contour)
9. symmetry
10. fractal dimension (“coastline approximation” - 1)
The variables are divided into three parts first is Mean (3-13), Stranded Error (13-23) and Worst (23-32) and each contain 10 parameters (radius, texture, area, perimeter, smoothness, compactness, concavity, concave points, symmetry and fractal dimension). Mean is the means of the all cells, standard Error of all cell and worst means the worst cell.

**Data Preprocessing**
This stage would include identifying if the data set contains any missing values or bad data.

**Modeling:**
After the usual ML pipeline with a train/test split of size 20% we train a CNN neural net with a binary cross-entropy loss of 0.0496 and accuracy 0.9805 on the train set against a loss of 0.0747 and accuracy 0.9737 on the test validation set. We confront predictions with the values on the test set and visualize the plots of the loss and the accuracy metrics on the train and test sets.

Resources and code used:
Python version: 3.7 Libraries/packages used: pandas, numpy, tensorflow, keras, scikitlearn
