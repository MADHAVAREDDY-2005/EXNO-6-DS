# EXNO-6-DS-DATA VISUALIZATION USING SEABORN LIBRARY
### Name : K MADHAVA REDDY
### Reg No : 212223240064
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
### Distribution plot:
```py
import seaborn as sns
import matplotlib.pyplot as plt
plt.figure(figsize=(6, 4))
sns.histplot(mod_df['price'], kde=True, color='blue')
plt.title('Distribution Plot - Price')
plt.show()
```
![image](https://github.com/user-attachments/assets/3405647e-9cd3-4783-bb9e-740d1f12cd83)
### KDE plot:
```py
plt.figure(figsize=(6, 4))
sns.kdeplot(mod_df['price'], shade=True, color='purple')
plt.title('KDE Plot - Price')
plt.show()
```
![image](https://github.com/user-attachments/assets/e6656b55-7ec1-4efa-a649-d6b990bd2adf)
### Pair plot:
```py
sns.pairplot(mod_df[['price', 'area', 'bedrooms', 'bathrooms', 'stories']])
plt.show()
```
![image](https://github.com/user-attachments/assets/531d6981-0f9f-40bb-8c6e-b07ccf86b0a9)
### Count plot:
```py
plt.figure(figsize=(15, 5))
plt.subplot(1, 3, 1)
sns.countplot(x='mainroad', data=mod_df)
plt.title('Count Plot - Mainroad')

plt.subplot(1, 3, 2)
sns.countplot(x='guestroom', data=mod_df)
plt.title('Count Plot - Guestroom')

plt.subplot(1, 3, 3)
sns.countplot(x='basement', data=mod_df)
plt.title('Count Plot - Basement')
plt.tight_layout()
plt.show()
```
![image](https://github.com/user-attachments/assets/ebd699c0-8c97-4cd3-a086-c87ea9c1c86c)
### Boxplot:
```py
plt.figure(figsize=(6, 5))
sns.boxplot(x='furnishingstatus', y='price', data=mod_df)
plt.title('Box Plot - Price vs Furnishing Status')
plt.show()
```
![image](https://github.com/user-attachments/assets/4378d277-09e2-4c29-a603-791589c387f7)
### Violin plot:
```py
plt.figure(figsize=(6, 5))
sns.violinplot(x='furnishingstatus', y='price', data=mod_df)
plt.title('Violin Plot - Price vs Furnishing Status')
plt.show()
```
![image](https://github.com/user-attachments/assets/55c36dd9-1fcb-40ea-9da8-be3180d11e25)

# Result:
Thus we have explored and applied every technique using seaborn successfully.
