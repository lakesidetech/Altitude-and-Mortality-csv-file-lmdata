# Altitude-and-Mortality-csv-file-lmdata
* * Manipualting and visualizing data with Python and core plotting libriaries Matplotlib and Seaborn
# import libraries
* import pandas as pd
* from pandas import DataFrame
* import numpy as np
* import matplotlib.pyplot as plt
* import seaborn as sns
* from statsmodels.formula.api import ols
* import statsmodels.api as sm

# 1: Load the data and print the column names
* * load data as a pandas dataframe and look at the columns
* df = pd.read_csv('/lmdata.csv')
* print (df)

![image](https://user-images.githubusercontent.com/17750481/113516988-05c6c100-9586-11eb-9cb8-866673fe4d7b.png)

# 2: Generate descriptive statistics for the data
## view some basic statistical details like percentile, mean, std,max,min,count of a data frame
df.describe()

![image](https://user-images.githubusercontent.com/17750481/113517180-1297e480-9587-11eb-9025-b418cedd7f10.png)

# 3: Create a line plot for the variables. Add a title and x & y axes.
    ![image](https://user-images.githubusercontent.com/17750481/113517257-7b7f5c80-9587-11eb-83a0-8502ea3d28da.png)
![image](https://user-images.githubusercontent.com/17750481/113518603-0401fb00-9590-11eb-904d-4db1303c647a.png)

# 4: Create a scatter plot / Add title and (X,Y) axis names
![image](https://user-images.githubusercontent.com/17750481/113517273-94880d80-9587-11eb-974b-19d62ca01a42.png)

# 5: Create a boxplot for mortality
![image](https://user-images.githubusercontent.com/17750481/113517295-b5506300-9587-11eb-973f-6fad033862e5.png)

# 6: Conduct a Pearson’s correlation test for the variables
![image](https://user-images.githubusercontent.com/17750481/113517306-c7ca9c80-9587-11eb-9d87-201eefc9b42d.png)

# 7: Create a pair plot for the data
![image](https://user-images.githubusercontent.com/17750481/113518135-02830380-958d-11eb-8460-b487c7e40f1d.png)

# 8: Create a Seaborn regplot of the regression model and a 95% confidence interval
![image](https://user-images.githubusercontent.com/17750481/113517413-78d13700-9588-11eb-86dd-95f87a4b192a.png)

# 10: Create the regression model using ols() from the statsmodel package
* * Now, let's prepare a simple linear model (OLS - for "ordinary least squares" method) with  latitude  as the response and mortality as the predictor:
* * type of linear least squares method for estimating the unknown parameters in a linear regression model
* lm = sm.OLS.from_formula('latitude ~ mortality', df)
 * result = lm.fit()
* #11: Print the model Summary
* print(result.summary())

# 11: Print the model Summary
* To get detailed information about the model
![image](https://user-images.githubusercontent.com/17750481/113517333-f2b4f080-9587-11eb-9974-138e08615c62.png)

