# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 02-05-2026

# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# ALGORITHM:
1. Import the required packages like pandas and matplot
2. Read the dataset using the pandas
3. Calculate the mean for the respective column.
4. Plot the data according to need and can be altered monthly, or yearly.
5. Display the graph.
# PROGRAM:
```
import pandas as pd
import matplotlib.pyplot as plt
df = pd.read_csv('Combined12.csv')
print(df.columns)
col = 'temp_mean(c)'
mean_value = df[col].mean()
print("Mean:", mean_value)
plt.figure(figsize=(10,5))
plt.plot(df.index, df[col], color='black', label='Temperature')
plt.title('Temperature Variation')
plt.xlabel('Index')
plt.ylabel('Temperature (C)')
plt.legend()
plt.grid()
plt.show()
```
# OUTPUT:

<img width="1062" height="577" alt="image" src="https://github.com/user-attachments/assets/3797d0db-69dc-48f6-b5af-0ae114712233" />



<img width="1057" height="516" alt="image" src="https://github.com/user-attachments/assets/fc062de3-8bc9-4ab6-b610-0d7f7d563239" />



# RESULT:
Thus we have created the python code for plotting the time series of given data.
