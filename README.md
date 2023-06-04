# Ex-09-Data-Visualization-

## AIM
To Perform Data Visualization on a complex dataset and save the data to a file. 

# Explanation
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# ALGORITHM
### STEP 1
Read the given Data
### STEP 2
Clean the Data Set using Data Cleaning Process
### STEP 3
Apply Feature generation and selection techniques to all the features of the data set
### STEP 4
Apply data visualization techniques to identify the patterns of the data.


# CODE
```
#DEVELOPED BY :Priyadharshini.P
#REGISTER NO:212222100039

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
tips_df=sns.load_dataset("tips")
tips_df
sns.barplot(data = tips_df,x = "total_bill",y = "day")
sns.relplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker", style = "smoker")
sns.displot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.barplot(data = tips_df,x = "total_bill", y="tip",hue = "smoker")
sns.kdeplot(data = tips_df, x ="total_bill", y = "tip", size ="size")
sns.relplot(data = tips_df, x ="total_bill", y = "tip", hue = "day", col = "time")
sns.relplot(data = tips_df, x = "total_bill",y = "tip", col="day",col_wrap=2)
sns.lineplot(x = "total_bill", y = "tip", data = tips_df, hue = "sex",
style = "sex",
markers = ["o","<"], legend = "auto")
```

# OUPUT

![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/549aa770-e480-4420-b554-363fb0e9007c)
![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/067f4404-7082-40d8-924b-d80d5e04747a)
![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/2a65dbfc-b7c9-4e7d-93f7-eb2766d4a6c2)

![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/5e0255f8-a4f9-46ee-8428-c1d593b71a9a)
![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/65db2413-8ebd-4a3c-a622-cd3a1c33e731)

![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/5734bcb2-dac7-4cf9-b791-d962614817a5)
![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/819afac2-7481-44ec-861a-364862232d67)

![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/f24237c8-f58b-4a44-800e-3fd589ef6495)
![image](https://github.com/Priyadharshini-Er/Ex-08-Data-Visualization_1/assets/119558093/c6be2afd-652d-4a92-899d-a5bd181fce43)

# RESULT
Thus Data Visualization is performed on the given dataset and save the data to a file.



















