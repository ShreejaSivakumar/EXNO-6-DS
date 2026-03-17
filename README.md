# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY

# NAME : SHREEJA R S
# REF.NO : 25017561
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
import seaborn as sns
```
```
import pandas as pd
df = pd.read_csv('iris.csv')
```
```
df.head()
```
<img width="704" height="581" alt="Screenshot 2026-03-17 214333" src="https://github.com/user-attachments/assets/f74eecda-935c-491b-a342-76f8ad7b7a19" />

```
df.corr()
```
```
sns.heatmap(df.corr())
```
<img width="1858" height="619" alt="Screenshot 2026-03-17 214355" src="https://github.com/user-attachments/assets/299bcc2e-99d0-4b7d-9230-06ccb5961fa9" />
<img width="829" height="606" alt="Screenshot 2026-03-17 214403" src="https://github.com/user-attachments/assets/7a3ae784-f36e-4a28-97c7-edc268d6ff43" />

```
sns.jointplot(x='sepal_length',y='petal_length',data=df,kind='hex')
```
<img width="863" height="848" alt="Screenshot 2026-03-17 214412" src="https://github.com/user-attachments/assets/03df7b23-61f1-4fd5-974f-ff74156e5fc4" />

```
sns.jointplot(x='sepal_length',y='petal_length',data=df,kind='reg')
```
<img width="884" height="844" alt="Screenshot 2026-03-17 214418" src="https://github.com/user-attachments/assets/a35c0ced-b0a6-41ee-9879-4914cd950476" />

```
sns.pairplot(df)
```
<img width="264" height="77" alt="Screenshot 2026-03-17 214427" src="https://github.com/user-attachments/assets/7f7276c6-055c-48d2-8d22-254f785c8ae2" />
<img width="649" height="638" alt="Screenshot 2026-03-17 214448" src="https://github.com/user-attachments/assets/a72641d3-9567-4b62-83c0-936405cb34bd" />

```
sns.pairplot(df,hue='species')
```
<img width="670" height="711" alt="Screenshot 2026-03-17 214458" src="https://github.com/user-attachments/assets/78f89d40-aa47-4829-a4f8-207a06f8a17f" />

```
sns.distplot(df['sepal_length'])
```
<img width="669" height="454" alt="Screenshot 2026-03-17 214504" src="https://github.com/user-attachments/assets/d56bbfc3-c870-4747-80e2-c917c4e3f4ca" />

```
sns.distplot(df['sepal_length'],kde=False,bins=10)
```

<img width="653" height="549" alt="Screenshot 2026-03-17 214509" src="https://github.com/user-attachments/assets/839380e2-a6c7-4cf0-bdf0-8e63d281d244" />

![Uploading Screenshot 2026-03-17 214517.png…]()
```
## Count plot

sns.countplot(x='species',data=df)
```
![Uploading Screenshot 2026-03-17 214524.png…]()

```
## Count plot

sns.countplot(y='species',data=df)
```

```
## Bar plot
sns.barplot(x='sepal_width',y='species',data=df)
```

```
## Bar plot
sns.barplot(x='species',y='sepal_width',data=df)
```


```
df.head()

```


```
sns.boxplot(x='sepal_length',y='petal_length', data=df)
```


```
sns.boxplot(x="sepal_width", y="petal_length", data=df,palette='rainbow')
```


```
sns.boxplot(data=df,orient='v')
```


```
# categorize my data based on some other categories

sns.boxplot(x="petal_length", y="petal_width", hue="sepal_length",data=df)
```

```
sns.violinplot(x="sepal_width", y="species", data=df,palette='rainbow')
```
![Uploading Screenshot 2026-03-17 214634.png…]()

# Result:
 Thus, Data Visualization using seaborn python library for the given datasets 
has been successfully performed.
