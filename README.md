This project was a personal project to practice using the Scikit-Learn library and XGBoost. 

In this project, I utilized the Wisconsin Breast Cancer dataset, this dataset comes from the University of Wisconsin-Madison.
The dataset contains the characteristics of a breast mass cell nuclei, the measurements are taken and computed by a digitized image of a fine
need aspirate (FNA). 
The classified variable is the Diagnosis variable containing two options: M = Malignant and B: Benign. 
In my analysis these two options were changedto 1 and 0, respectively. 

The first steps taken when performing Exploratory Data Analysis (EDA), was to normalize the data for each attribute (excluding the "Diagnosis" variable). 
This was done by creating a Normalization function and using the normalization function of (X - Xmin) / (Xmax - Xmin)

After normalization, an 80/20 train/test split was created to train the model.

Using the training split, a Hyperparamter tuning function was created, this function utilizes the Sci-Kit learn module GridSearchCV to perform a grid
search on possible parameters. After the grid search was completed the best parameters with an rmse of 3.21e-05, included n_estimators: 100, colsample_bytree: 1.0,
learning_rate: 0.5, max_depth: 3, sub_sample: 0.6.


