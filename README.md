This project is a small data preprocessing exercise using the Titanic dataset. The main goal was to clean the data, handle missing values, convert categorical columns into numerical form, remove outliers, and prepare the dataset so it’s ready for machine learning models.

1. Loaded the dataset
I started by importing the Titanic dataset into a pandas DataFrame and checked the first few rows and basic information. This helped me understand the structure of the data and see which columns needed cleaning.

2. Handled missing values
Some columns had missing data, so I filled them using simple methods like mean or median imputation. After fixing the missing values, I ran df.info() again to make sure everything was updated correctly.

3. Dropped unnecessary columns
Certain columns weren’t very useful for modeling (like PassengerId, Name, and in some cases Ticket/Cabin). I removed them to keep the dataset clean and focused.

4. Encoded categorical features
Columns like Sex and Embarked were categorical, so I converted them into numeric form using one-hot encoding (get_dummies). This makes the data compatible with machine learning algorithms.

5. Scaled the numerical data
I used StandardScaler to standardize the numeric features. This ensures that all the numbers are on a similar scale, which usually improves model performance.

6. Checked and removed outliers
I plotted a boxplot for the Fare column to identify outliers. Based on the visualization and the distribution, I removed extreme values so they wouldn’t negatively affect future models.

7. Prepared the final cleaned dataset
After all these steps—cleaning, encoding, scaling, and outlier removal—I ended up with a cleaned and fully preprocessed dataset that’s ready for model training.
