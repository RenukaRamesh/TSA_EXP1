# Ex.No: 01A PLOT A TIME SERIES DATA
###  Date: 03.02.2026
### Name: Ramesh Renuka
### Reg.no: 212223240136
# AIM:
To Develop a python program to Plot a time series data (population/ market price of a commodity
/temperature.
# SOFTWARE REQUIRED:
Google Colab
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
df=pd.read_csv('/content/retail_sales_dataset.csv')

df.info()
df = df.sort_values('Date')
plt.plot(df['Date'], df['Total Amount'], marker='o')
plt.xlabel("Date")
plt.ylabel("Total Amount")
plt.title("Total Amount over Date")
plt.grid(True)
plt.show()

df['Date'] = pd.to_datetime(df['Date'])
df = df.sort_values('Date')

plt.plot(df['Date'], df['Price per Unit'])
plt.xlabel("Date")
plt.ylabel("Price per Unit")
plt.title("Price per unit over Date")
plt.grid(True)
plt.show()
```
# OUTPUT:
<img width="1030" height="399" alt="image" src="https://github.com/user-attachments/assets/52f1f85f-c960-4d2b-9608-dfeae3a37997" />

<img width="579" height="342" alt="image" src="https://github.com/user-attachments/assets/d1127efc-3781-4ef2-a667-5fe50c1c5552" />

<img width="771" height="644" alt="image" src="https://github.com/user-attachments/assets/3eb7ba89-3002-4115-b900-34ec6569a9a0" />

<img width="722" height="682" alt="image" src="https://github.com/user-attachments/assets/eed89377-6501-4de9-a55f-b7d77b0eede4" />


# RESULT:
Thus we have created the python code for plotting the time series of given data.
