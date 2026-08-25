# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

## Line Plot
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
marks=[13,45,63,78]
student=['ABC','QOR','EFB','TOB']
plt.plot(marks,student)
plt.xlabel('Marks')
plt.ylabel('Student name')
plt.show()
student=['A','B','C','D']
attendence=[90,85,73,88]
plt.plot(attendence,student)
plt.xlabel('Attendence')
plt.ylabel('Student name')
plt.show()
```
<img width="847" height="534" alt="image" src="https://github.com/user-attachments/assets/9355f5eb-5da2-423a-8dda-3daf4ad85538" />
<img width="854" height="562" alt="image" src="https://github.com/user-attachments/assets/79dfe188-59f5-41a5-be7f-8195acf2bdb0" />

## Scatter Plot
```
x=[10,20,30,40,50]
y=[100,200,300,400,500]
plt.scatter(x,y,label='stars',color='green',marker='*',s=30)
plt.show()
x=np.arange(0,15)
y=np.arange(0,15)
x
y
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('y axis')
plt.title('Scatter plot')
plt.show()
```
<img width="726" height="527" alt="image" src="https://github.com/user-attachments/assets/b2473136-c35e-468e-bb60-f62e7e6f451d" />
<img width="757" height="567" alt="image" src="https://github.com/user-attachments/assets/5b106abd-621b-4932-ac27-1bb60927434d" />

## Pie Chart
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
color=['r','y','g','b']
plt.pie(slices,labels=act,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
feedback=['Good','excellent','Perfect','Ok']
slices=[4,10,3,8]
color=['y','r','b','g']
plt.pie(slices,labels=feedback,colors=color,startangle=90,shadow=True,explode=(0.1,0.1,0.1,0.1),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
<img width="697" height="513" alt="image" src="https://github.com/user-attachments/assets/06fcf709-c4fc-4fe1-a049-58f635be4f13" />
<img width="647" height="531" alt="image" src="https://github.com/user-attachments/assets/44cb17cb-bad8-4714-bee9-265187dc813d" />

## Area Chart
```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='green')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='black')
plt.legend(['y1','y2'])
plt.show()
```
<img width="722" height="520" alt="image" src="https://github.com/user-attachments/assets/62997ce0-de5e-442c-abc2-6817043ef4be" />

## Bar Chart
```
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('My bar chart!')
plt.show()
```
<img width="736" height="558" alt="image" src="https://github.com/user-attachments/assets/4d3568c9-ba32-497e-b80e-1cc362137d80" />

## Histogram
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
<img width="702" height="513" alt="image" src="https://github.com/user-attachments/assets/d36c3c4d-a3a6-4062-b853-34e25780e033" />

## Box Plot
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="828" height="445" alt="image" src="https://github.com/user-attachments/assets/f4cf4ca9-1b7b-4ec9-aaba-02a7ac5d31d8" />

```
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
<img width="844" height="602" alt="image" src="https://github.com/user-attachments/assets/10441fee-96e5-4f71-a5e3-4c176b5f4e5e" />

# Result:
Thus, all the data visualization techniques of matplotlib has been implemented.
