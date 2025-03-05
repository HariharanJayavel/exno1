# Exno:1
Data Cleaning Process

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
df = pd.read_csv("/content/SAMPLEIDS.csv")
df
```
![image](https://github.com/user-attachments/assets/459a437e-d1b2-4d9f-bf93-d45afee50ce1)
```
df.head()
df.tail()
```
![image](https://github.com/user-attachments/assets/f4842f18-547a-49bb-9469-6f066ed7a219)

![image](https://github.com/user-attachments/assets/2c9f1f3f-ba0d-4595-9db6-fb642cad8da4)

```
df.isnull().sum()
```
![image](https://github.com/user-attachments/assets/bd1c88ff-f725-46f7-99cb-40318b820674)
```
df.isnull().any()
```
![image](https://github.com/user-attachments/assets/3b9942e0-be1d-4b9d-ad9b-e0c28c2b67ca)
```
df.dropna(axis = 0)
```
![image](https://github.com/user-attachments/assets/3d298ecf-b68c-4939-98d8-8c7a422fedf0)
```
df.dropna(axis=1)
```
![image](https://github.com/user-attachments/assets/08697b09-da18-4949-ba7d-03e252b97eae)
```
df.fillna(method = 'ffill')
```
![image](https://github.com/user-attachments/assets/6ebeec00-ddfd-47c4-a898-c47a5724fa20)
```
df.fillna(method = 'bfill')
```
![image](https://github.com/user-attachments/assets/7d043470-9144-444b-9378-ed188ac7bd91)
```
df_dropped = df.dropna()
df_dropped
```
![image](https://github.com/user-attachments/assets/6e1fe0ef-1196-44d4-a260-124cb835bc88)
```
![image](https://github.com/user-attachments/assets/38c5dd5b-816b-4a1b-8e39-8fd768e36420)
```
![image](https://github.com/user-attachments/assets/b10ec7b5-79b3-4c4c-b9af-348ed599c759)
```
data = pd.read_csv("/content/iris.csv")
data
```
![image](https://github.com/user-attachments/assets/eb583e17-144e-443e-b4be-192c26a9e6f2)
```
data.describe()
```
# Result
          <<include your Result here>>
