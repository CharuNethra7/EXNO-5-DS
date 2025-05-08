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
### Register No.: 212223230035
### Developed By: CHARU NETHRA R
```
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
plt.plot(x,y,label='line1')
```
![1](https://github.com/user-attachments/assets/692cedca-bc58-4be6-93a6-fce50fb6de48)


```
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]

plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```

![2](https://github.com/user-attachments/assets/22964f1c-a990-4e93-9f2c-a36588bb94a5)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
```
![3](https://github.com/user-attachments/assets/32102036-5ce7-431c-b43d-564cd900201a)


```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![4](https://github.com/user-attachments/assets/0dbfc2df-7632-4afc-9100-d446b96c206a)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![5](https://github.com/user-attachments/assets/a6a5da9e-2d00-4dcb-a090-82611b7057ea)


```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
```
![6](https://github.com/user-attachments/assets/fd40fcf8-e56d-4243-b35b-688db0c26d00)


```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![7](https://github.com/user-attachments/assets/049ebbd9-6bb1-47dc-93e2-54f717c98d19)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```

![8](https://github.com/user-attachments/assets/8c13e4c7-8ed8-434a-a77e-cb88f64f3dc9)


```
y
```
![9](https://github.com/user-attachments/assets/01e727db-e7b2-4e01-8aa6-ddd7ab6072aa)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![10](https://github.com/user-attachments/assets/b8ce927c-8990-40d3-8f0c-d65f7718b4bd)



```
y=x*x
y
```
![11](https://github.com/user-attachments/assets/dd89cd69-6be9-4cb6-987d-854f280a6046)


```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
```
![12](https://github.com/user-attachments/assets/c06724c9-190a-4a33-9072-2659b1afe408)


```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![13](https://github.com/user-attachments/assets/8f2d5212-740f-4aa4-baee-34fab61653af)


```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
```
![14](https://github.com/user-attachments/assets/3d5d995f-2ebf-42ad-8271-cc5b92a60bf3)


```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')

plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![15](https://github.com/user-attachments/assets/3f2a2c9d-fb99-444a-9144-5839d237aa0c)


```
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
```
![16](https://github.com/user-attachments/assets/596f0c35-0a81-45b1-a029-60f2d7467cb2)


```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
```
![17](https://github.com/user-attachments/assets/001d5cae-e951-4e09-84f0-38bd304e000d)


```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
```
![18](https://github.com/user-attachments/assets/0c4f2d1c-2f40-4f2c-be43-15c9f24fa702)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![19](https://github.com/user-attachments/assets/7c581646-c02a-4793-a007-8855317a2fff)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![20](https://github.com/user-attachments/assets/f62045b6-6720-4dc5-8364-1a8633d32ddb)


```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```

![21](https://github.com/user-attachments/assets/27ad4acf-e6e7-4f11-9a1a-377f54046528)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![22](https://github.com/user-attachments/assets/3efa67f1-a12c-4a66-a260-9198576168f2)

# Result:
Thus, The implementation of data visualization using matplotlib has been successfully verified.
