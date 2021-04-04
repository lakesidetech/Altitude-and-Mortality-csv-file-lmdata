# Altitude-and-Mortality-csv-file-lmdata
Generate descriptive statistics for the data using Numpy, pandas, Python, and Seaborn
# 1: Load the data and print the column names
* 1: Load the data and print the column names
* df = pd.read_csv('/lmdata.csv')
* print (df)

![image](https://user-images.githubusercontent.com/17750481/113516988-05c6c100-9586-11eb-9cb8-866673fe4d7b.png)

# 2: Generate descriptive statistics for the data
## view some basic statistical details like percentile, mean, std,max,min,count of a data frame
df.describe()

![image](https://user-images.githubusercontent.com/17750481/113517180-1297e480-9587-11eb-9025-b418cedd7f10.png)

# 3: Create a line plot for the variables. Add a title and x & y axes.
    ![image](https://user-images.githubusercontent.com/17750481/113517257-7b7f5c80-9587-11eb-83a0-8502ea3d28da.png)

# 4: Create a scatter plot / Add title and (X,Y) axis names
![image](https://user-images.githubusercontent.com/17750481/113517273-94880d80-9587-11eb-974b-19d62ca01a42.png)

# 5: Create a boxplot for mortality
![image](https://user-images.githubusercontent.com/17750481/113517295-b5506300-9587-11eb-973f-6fad033862e5.png)

# 6: Conduct a Pearson’s correlation test for the variables
![image](https://user-images.githubusercontent.com/17750481/113517306-c7ca9c80-9587-11eb-9d87-201eefc9b42d.png)

# 7: Create a pair plot for the data

# Create the default pairplot
# 8: Type in this command: from statsmodels.formula.api import ols
# 9: Create a Seaborn regplot of the regression model and a 95% confidence interval
# plot the regression model y ~ x and a 95% confidence interval for that regression
# 10: Create the regression model using ols() from the statsmodel package
# 11: Print the model Summary
