# BreastCancer

**Introduction** 
Breast cancer is a malignant cell growth in the breast. If left untreated, the cancer spreads to other areas of the body. Excluding skin cancer, breast cancer is the most common type of cancer in women in the United States, accounting for one of every three cancer diagnoses. Breast cancer ranks second among cancer deaths in women. This project aims at analyzing data of women residing in the state of Wisconsin, USA for to predict whether a case of breast cancer is malignant or benign.

**Problem statement**
The goal of this project is the application of several data mining and machine learning techniques to classify whether the tumor mass is benign or malignant in women residing in the state of Wisconsin, USA. This will help in understanding the important underlaying importance of attributes thereby helping in predicting the stage of breast cancer depending on the values of these attributes. Through the understanding of nature of attributes in cancer prediction, the healthcare community can perform additional research corresponding to these attributes to help prevent pervasion of breast cancer into the population of USA.

**Assumption and scope**
The project assumes that the dataset collected is representative of the entire women population of Wisconsin, USA. . The data has been collected accurately . No errors have been committed while entering the collected data

The scope of the project is confined only to prediction of breast cancer to be malignant or benign for the women of Wisconsin. This project will not include any conclusions that can be made whatsoever for the remaining women population of USA. The project will not go in depths of the reason whatsoever of the greater importance of some attributes over that of other attributes in prediction of breast cancer cases, as this would require considerable domain expertise in biomedical sciences.

**Data cleaning and preparation**
This stage would include identifying if the data set contains any missing values or bad data. I would the convert the diagnosis (Y variable) into appropriate format (currently it is classified as M and B for malignant and benign respectively)

**Exploratory data analysis**
The EDA process will help in understanding the nature of the dataset and help in identification of potential outliers or correlated variables.

**modelling overview**
For modelling, K-nearest neighbor, random Forest and Support Vector Machine algorithms would be used for classification of the diagnosis Y-variable in the data as malignant or benign. The data will be portioned into training and test sets, consisting of 80% and 20% of the original data respectively. These models would be built on training dataset and testing dataset would be used for testing model performance.

**Dataset**
data is taken from:- https://archive.ics.uci.edu/ml/datasets/Breast+Cancer+Wisconsin+%28Diagnostic%29

Features in the dataset are computed from a digitized image of a fine needle aspirate (FNA) of a breast mass. Separating plane described above was obtained using Multisurface Method-Tree (MSM-T) [K. P. Bennett, “Decision Tree Construction Via Linear Programming.” Proceedings of the 4th Midwest Artificial Intelligence and Cognitive Science Society, pp. 97-101, 1992], a classification method which uses linear programming to construct a decision tree. Relevant features were selected using an exhaustive search in the space of 1-4 features and 1-3 separating planes. The dataset contains information of 569 women across 32 different attributes. 1) ID number 2) Diagnosis (M = malignant, B = benign)

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
