# Exno:1 Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
import pandas as pd
data=pd.read_csv("SAMPLEIDS.csv")
data
```
![image](https://github.com/user-attachments/assets/0b733593-c624-4940-8293-65d05ff45229)
```
data.head()
```
![image](https://github.com/user-attachments/assets/06e1ddde-b8bc-4677-967f-529191dbe4d3)
```
data.tail()
```
![image](https://github.com/user-attachments/assets/e3d3b29f-b562-4ff1-850b-5567d2ba7db6)
```
data.isnull()
```
![image](https://github.com/user-attachments/assets/f608e511-86ee-44ec-8421-74e348021caa)
```
data.isnull().sum()
```
![image](https://github.com/user-attachments/assets/eb27fd60-5d41-44bf-8828-ce9ea32973f0)
```
data.isnull().any()
```
![image](https://github.com/user-attachments/assets/09506df2-ef07-4611-8a29-d72c10b716e9)
```
data.dropna()
```
![image](https://github.com/user-attachments/assets/64c85113-58ad-4c1e-9586-d6f99a422216)
```
data.fillna(0)
```
![image](https://github.com/user-attachments/assets/46002150-0be6-4187-b025-d83690429907)
```
data.fillna(method='ffill')
```
![image](https://github.com/user-attachments/assets/8a8b8595-db29-4ac1-93d5-eb114d19487b)
```
data.fillna(method='bfill')
```
![image](https://github.com/user-attachments/assets/ec229a15-0a80-4374-bcf9-97679e3e50e7)
```
 data.fillna({'GENDER':'MALE','NAME':'SRI','ADDRESS':'POONAMALEE','M1':98,'M2':87,'M3':76,'M4':92,'TOTAL':305,'AVG':89.999999})
```
```
import pandas as pd
ir=pd.read_csv("iris.csv")
ir
```

# Result
          <<include your Result here>>
