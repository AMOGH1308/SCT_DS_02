# Titanic Dataset Analysis

This repository contains a detailed analysis of the Titanic dataset, focusing on Data Cleaning and Exploratory Data Analysis (EDA).

## Data Cleaning Process

1. **Loading the Dataset:**
   - The dataset was loaded into a Pandas DataFrame using the `read_csv()` function.
   
2. **Selecting First 100 Samples:**
   - We used the `head()` function to select the first 100 samples from the dataset for analysis.

3. **Handling Missing Values:**
   - Checked for null values using `isnull().sum()`.
   - Dropped duplicates, if any.
   - Removed the `Cabin` column due to a large number of missing values.
   - Filled missing values in the `Age` column with the median value of the column.
   - Filled missing values in the `Embarked` column using the mode (most frequent value).

4. **Categorical Variable Encoding:**
   - Converted string values in categorical variables like `Sex` and `Embarked` into numerical values (e.g., 0, 1) for analysis purposes.

5. **Cleaning `Ticket` Column:**
   - Removed non-numeric values in the `Ticket` column.

6. **Dropping Unnecessary Columns:**
   - The `Name` column was removed to simplify the analysis.

## Exploratory Data Analysis (EDA)

1. **General Information:**
   - The `info()` method was used to display data types and the number of non-null values in each column.
   
2. **Descriptive Statistics:**
   - The `describe()` method provided statistical insights such as mean, count, minimum, and maximum for numeric columns.

3. **Correlation Analysis:**
   - A correlation matrix was calculated and visualized using a heatmap to examine relationships between different numerical features.

4. **Univariate Analysis:**
   - Plotted histograms for variables like `Age` and `Fare` to understand their distribution and frequency.

5. **Categorical Variable Distribution:**
   - Analyzed variables like `Sex`, `Survived`, and `Pclass` to observe the frequency of each value.

6. **Bivariate Analysis:**
   - **Sex vs. Survived:** To analyze survival rates based on gender.
   - **Pclass vs. Survived:** To examine which passenger class had higher survival rates.

## Trends and Patterns

1. **Age Distribution:**
   - Most passengers were young, aged between 20-30 years.
   
2. **Fare Distribution:**
   - Many passengers paid a fare between 0-50 for their trip.

3. **Gender Distribution:**
   - Males were more in number compared to females.

4. **Survival Rate:**
   - More people perished in the disaster than survived.
   
5. **Passenger Class Distribution:**
   - The third class had the highest number of passengers.
   
6. **Gender Survival Rate:**
   - Females had a higher survival rate compared to males.

7. **Class Survival Rate:**
   - Passengers in the second class (moderate class) had a higher survival rate compared to other classes.

## Conclusion

Through this analysis, we gained insights into the demographics and survival trends of passengers on the Titanic. The findings highlight key factors such as age, fare, gender, and class in determining survival likelihood.

      
