![image](https://github.com/user-attachments/assets/77e2ccbe-58b1-4b6b-9e09-55371cbae625)# EXNO2DS
# AIM:
      To perform Exploratory Data Analysis on the given data set.
      
# EXPLANATION:
  The primary aim with exploratory analysis is to examine the data for distribution, outliers and anomalies to direct specific testing of your hypothesis.
  
# ALGORITHM:
STEP 1: Import the required packages to perform Data Cleansing,Removing Outliers and Exploratory Data Analysis.

STEP 2: Replace the null value using any one of the method from mode,median and mean based on the dataset available.

STEP 3: Use boxplot method to analyze the outliers of the given dataset.

STEP 4: Remove the outliers using Inter Quantile Range method.

STEP 5: Use Countplot method to analyze in a graphical method for categorical data.

STEP 6: Use displot method to represent the univariate distribution of data.

STEP 7: Use cross tabulation method to quantitatively analyze the relationship between multiple variables.

STEP 8: Use heatmap method of representation to show relationships between two variables, one plotted on each axis.

## CODING AND OUTPUT
NAME: JEGATHEESWARI R
REG NO: 212223230092
```
import pandas as pd
df=pd.read_csv("/content/titanic_dataset.csv")
df
![Screenshot 2024-09-03 220639](https://github.com/user-attachments/assets/25ac95e0-a321-4665-9b56-91f6c2592762)
```
```
df.isnull().sum()
![Screenshot 2024-09-03 220803](https://github.com/user-attachments/assets/e5bd2dde-c81a-4ce7-bccd-3a4dbcccc439)
```
```
df.dropna(inplace=True)
df
![Screenshot 2024-09-03 220924](https://github.com/user-attachments/assets/666942b3-a36c-4a35-80ff-e3eddb072f30)
```
```
df.info()
![Screenshot 2024-09-03 221008](https://github.com/user-attachments/assets/0f4a3dee-a6e8-42a8-8905-e3697efe4c31)
```
```
df.shape
![Screenshot 2024-09-03 221038](https://github.com/user-attachments/assets/f53c437d-f807-4add-883c-1a3d0bd1941f)
```
```
df.set_index("PassengerId",inplace=True)
df
![Screenshot 2024-09-03 221115](https://github.com/user-attachments/assets/4af46c78-09e2-4648-aa9a-ab4462c9ff23)
```
```
df.nunique()
![Screenshot 2024-09-03 221153](https://github.com/user-attachments/assets/8f0f7789-ec50-458c-845b-6e1b405f04d5)
```
```
df["Survived"].value_counts()
![Screenshot 2024-09-03 221222](https://github.com/user-attachments/assets/116a2986-6cea-4ca3-af6d-50f3047150ea)

```
```
per=(df["Survived"].value_counts()/df.shape[0]*100).round(2)
per
![Screenshot 2024-09-03 221246](https://github.com/user-attachments/assets/08b1c924-9051-44e2-a03f-b32d01ba3f8a)
```

# RESULT
        <<INCLUDE YOUR RESULT HERE>>
