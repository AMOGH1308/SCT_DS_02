Data cleaning and Exploratory Data Analysis(EDA) on a Titanic Dataset from Kaggle.

Data Cleaning:-
->first we load the csv file into a dataframe
->we take only the first 100 samples of data in a dataset using the head() function
->we check if there are any null values
->if we drop any duplicates present in the dataframe
->we remove 'cabin' column from the dataframe because most of its values are Nan values and it is not useful for our further analysis part.
->in the 'Age' column we fill the Nan values with the median value of all the values present in the age column.
->in the 'Embarked' column the Nan values are filled using the mode() function(i.e it is filled with the most commonly reccuring values in that column).
->we replace all the string values present in categorial variables such as sex and embarked with Numeric values(such as 0,1..etc) so that we can determine the distribution of each of these column which is required for the analytical part.
->we remove any non-numeric values present in the column 'Ticket' column.
->we drop the 'Name' column from the dataframe to make the dataframe ready for further EDA.

Exploratory Data Analysis(EDA):-
->we use the info() method to gather information of all the columns such as the dtype of all the columns,no of non-null values present in each column.
->we use the describe() method to calculate various parameters such as mean,count,min etc.. of each column.
->we determine the correlation matrix of the whole dataset and we display the whole corr matrix in the form of a heatmap plot.
->then we find the distribution of univariate variables such as 'age','Fare' and we find the frequency of each of the these columns values individually using histogram plot.
->distribution of categorial vairables such as 'sex','Survived','Pclass' to determine the frequency of each of their values
->distribution of Bivariate variables such as:-
      1). sex and Survived:-to determine which particular gender had a higher survival rate.
      2). Pclass and Survived:-to determine the people in which passenger class(such as high,moderate or low class) had a higher survival rate.

Trends and Patterns:-
After a detailed Analysis of the first 100 data samples in a Dataframe we came to a Know that:-
    1). most of the people in the ship were young individuals between the age of 20-30
    2). many of them paid a fare of somewhere between 0-50 for their trip
    3). males were more compared to females
    4). no of people who died in this tragic incident is greater than the ones who survived
    5). there were more people from the 3rd class compared to the other two classes.
    6). females have a higher survival rate compared to males
    7). the 2nd class(moderate class) had higher survival rate compared to the people under other classes
      
