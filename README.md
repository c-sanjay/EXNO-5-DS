# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## Aim:
  To Perform Data Visualization using matplot python library for the given datas.

## EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

## Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

## Coding and Output:
```
NAME: SANJAY C
REG NO: 212223240150
```
```py
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
```

### Line Plot:

```py
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

<img width="730" height="533" alt="image" src="https://github.com/user-attachments/assets/4653bd5c-775e-4fe8-9e75-1bc0b4cb6aff" />
<img width="737" height="539" alt="image" src="https://github.com/user-attachments/assets/ff982eef-3a08-4b75-bcfb-77b56885b746" />

### Scatter Plot:

```py
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

<img width="716" height="510" alt="image" src="https://github.com/user-attachments/assets/5bda3f3e-f8b3-4ba2-955e-2c4793d1b13f" />
<img width="722" height="547" alt="image" src="https://github.com/user-attachments/assets/df35ccac-6844-4f06-86b4-fe485a117e97" />


### Pie Chart:

```py
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


<img width="669" height="546" alt="image" src="https://github.com/user-attachments/assets/7fdb5405-0337-4dbc-b70a-3c6213a6c35e" />
<img width="597" height="502" alt="image" src="https://github.com/user-attachments/assets/676d82ae-0523-443f-8be7-346a90d466d6" />


### Area Chart:

```py
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]
y3 = [2, 4, 6, 8, 10]
plt.fill_between(x, y1, color='blue')
plt.fill_between(x, y2, color='red')
plt.plot(x, y1, color='red')
plt.plot(x, y2, color='yellow')
plt.legend(['y1','y2'])
plt.show()
```

<img width="707" height="500" alt="image" src="https://github.com/user-attachments/assets/73a46678-491d-4063-aa56-bf7f55a926a2" />



### Bar Chart:

```py
height = [10, 24, 36, 40, 5]
names = ['one', 'two', 'three', 'four', 'five']
c1=['red', 'green'] 
c2=['b', 'g']
plt.bar (names, height, width=0.8, color=c1)
plt.xlabel('x - axis')
plt.ylabel('y - axis')
plt.title('Bar chart')
plt.show()
```

<img width="749" height="552" alt="image" src="https://github.com/user-attachments/assets/586cd4a0-a8d7-414a-86f9-0643c1c7c423" />



### Histogram:

```py
x = [2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x, bins = 10, color='Yellow', alpha=0.5)
plt.show()
```


<img width="689" height="497" alt="image" src="https://github.com/user-attachments/assets/774cb5e6-acbd-4186-a802-6cd9219d4725" />



### Box Plot:

```py
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```


<img width="702" height="437" alt="image" src="https://github.com/user-attachments/assets/180b1224-dac9-4e6e-ba27-0fe779038909" />


```py
fig, ax= plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```

<img width="724" height="586" alt="image" src="https://github.com/user-attachments/assets/e7ab2781-a8f4-426a-b0c0-fbb77086a72b" />





## Result:

Thus, all the data visualization techniques of matplotlib has been implemented.
