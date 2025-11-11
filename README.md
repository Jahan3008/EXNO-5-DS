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
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```
## Line Plot:
```
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
<img width="748" height="536" alt="Screenshot 2025-10-29 133715" src="https://github.com/user-attachments/assets/0b4b6822-60ef-486a-a04d-42d854c871d3" />

<img width="733" height="545" alt="image" src="https://github.com/user-attachments/assets/f6a18474-46c7-47a5-abc9-58c7f9ff507f" />

##  Scatter Plot:
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

<img width="905" height="864" alt="Screenshot 2025-10-29 133817" src="https://github.com/user-attachments/assets/09c2f43f-d191-4f0e-9e9c-39402fb90ec3" />

<img width="718" height="527" alt="image" src="https://github.com/user-attachments/assets/a045f343-fa46-43f5-812a-9d400a69dda5" />

## Pie Chart:
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
<img width="1357" height="837" alt="Screenshot 2025-10-29 133849" src="https://github.com/user-attachments/assets/c5439388-528c-4b9f-8267-4d1d326cc8eb" />

<img width="615" height="528" alt="Screenshot 2025-10-29 133903" src="https://github.com/user-attachments/assets/b252397f-2ed9-443a-832c-b0f47a9ebf47" />

##  Area Chart:

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

<img width="837" height="792" alt="image" src="https://github.com/user-attachments/assets/f95081a6-02a5-480c-aedc-2a1a5ca3c084" />

##  Bar Chart:

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

<img width="885" height="830" alt="Screenshot 2025-10-29 133934" src="https://github.com/user-attachments/assets/4d6b6f6f-6fa4-4801-93c0-bc3ec51fc472" />

##  Histogram:
```
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='blue', alpha=0.5)
plt.show()
```
<img width="791" height="631" alt="Screenshot 2025-10-29 133946" src="https://github.com/user-attachments/assets/659fb297-3245-44e9-914b-6b9234cf3264" />

## Box Plot:
```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```
<img width="823" height="551" alt="image" src="https://github.com/user-attachments/assets/bc627f35-9c39-4d5b-9b12-6611e2030c0f" />

```
 fig, ax= plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')
```
<img width="904" height="759" alt="Screenshot 2025-10-29 134006" src="https://github.com/user-attachments/assets/902e0104-1933-4b67-ad99-9ab48494bd6a" />


# Result:
 Thus, all the data visualization techniques of matplotlib has been implemented.
