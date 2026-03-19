# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY
## NAME : PRANAV S
## RGISTER NUMBER : 212224040242
# Aim:
  To Perform Data Visualization using seaborn python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:
```
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 df=pd.read_csv("titanic_dataset.csv")
 df.head()
```
 <img width="1543" height="278" alt="image" src="https://github.com/user-attachments/assets/8d94d7f1-99b5-4ca9-8f27-7d58fba725a4" />

```
 x=[1,2,3,4,5]
 y=[3,6,2,7,1]
 sns.lineplot(x=x,y=y)
 plt.title('Line Plot')
```
 <img width="737" height="634" alt="image" src="https://github.com/user-attachments/assets/684dc5b0-3985-40c6-8a68-c7fb565d89b2" />

```
 x=[1,2,3,4,5]
 y1=[3,5,2,6,1]
 y2=[1,6,4,3,8]
 y3=[5,2,7,1,4]
 sns.lineplot(x=x,y=y1)
 sns.lineplot(x=x,y=y2)
 sns.lineplot(x=x,y=y3)
 plt.title('Multi Line Plot')
```
 <img width="740" height="637" alt="image" src="https://github.com/user-attachments/assets/8f079162-9957-48dc-ae8a-2b11bb85516a" />

```
 plt.figure(figsize=(8,5))
 sns.barplot(x='Embarked',y='Fare',data=df,palette='rainbow')
 plt.title("Fare Of Passenger By Embarked Town")
```
 <img width="1591" height="726" alt="image" src="https://github.com/user-attachments/assets/b74b0662-23f8-461c-bf5d-cec2091a8e5c" />

```
 sns.scatterplot(x="Age", y="Fare", data=df)
 plt.title('Scatterplot of Age vs Fare')
 plt.show()

 
 sns.scatterplot(x="Age", y="Fare", size="Pclass", data=df, sizes=(30, 200))
 plt.title('Bubble Chart of Age vs Fare, Size by Passenger Class')
 plt.show()
```
 <img width="711" height="570" alt="image" src="https://github.com/user-attachments/assets/e83557e8-e223-4a1a-a6aa-5a9dc1929b0d" />

```
 sns.histplot(data=df,x="Pclass",hue="Survived",kde=True)
```
 <img width="717" height="563" alt="image" src="https://github.com/user-attachments/assets/f3d78e1f-e96c-4f68-a45f-b9f09f16165c" />

```
 sns.boxplot(x='Pclass',y='Age',data=df,palette='rainbow')
 plt.title("Age By Passenger Class")
```
 <img width="1604" height="709" alt="image" src="https://github.com/user-attachments/assets/5e21300e-562e-400b-a3b2-8b2c3023304f" />

```
 sns.violinplot(x="Pclass", y="Fare", data=df)
 plt.title('Violin Plot of Fare by Passenger Class')
 plt.show()
```
 <img width="710" height="561" alt="image" src="https://github.com/user-attachments/assets/10caf32b-f4aa-47e8-88db-fe4e54fad7bc" />

```
 sns.kdeplot(data=df['Age'], shade=True)
 plt.title('Density Plot of Passenger Ages')
 plt.show()
```
 <img width="733" height="715" alt="image" src="https://github.com/user-attachments/assets/0db80a73-f8ab-4564-b160-76df1f40384d" />

```
 numeric_df = df.select_dtypes(include=['float64', 'int64'])
 corr_matrix = numeric_df.corr()
 sns.heatmap(corr_matrix, annot=True, cmap='coolwarm')
 plt.title('Heatmap of Titanic Dataset')
 plt.show()
```
 <img width="740" height="623" alt="image" src="https://github.com/user-attachments/assets/f80919d0-add6-418d-9de9-1cbe5b711125" />

# Result:
Data Visualization using seaborn python library for the given datas is performed successfully.
