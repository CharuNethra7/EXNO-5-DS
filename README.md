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
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
 plt.plot(x,y,label='line1')
```
![image](https://github.com/user-attachments/assets/249bdea8-2077-4adb-9f92-a0867f760e49)
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
![image](https://github.com/user-attachments/assets/eaf036e7-665e-4800-bd2c-1790948f56ec)
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
![image](https://github.com/user-attachments/assets/6dc8b46c-8291-4aab-a27b-8ed178c4d7f9)
```
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(yield_apples)
```
![image](https://github.com/user-attachments/assets/e9606cf7-d4fe-49ff-aa86-9c1262f34d23)
```
 years=[2010,2011,2012,2013,2014,2015]
 yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
 plt.plot(years,yield_apples)
```
![image](https://github.com/user-attachments/assets/c53f9875-a64d-447d-b9e6-eebafb117dac)
```
 years=range(2000,2012)
 apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
 oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
 plt.plot(years, apples)
 plt.plot(years, oranges)
 plt.xlabel('Year')
 plt.ylabel('Yield (tons per hectare)')
 plt.title('Crop Yields in Kanto')
 plt.legend(['Apples','Oranges'])
```
![image](https://github.com/user-attachments/assets/5b1898c6-69ae-4501-85b9-cfd9c824e1bc)
```
 plt.figure(figsize=(12,6))
 plt.plot(years,oranges,marker='o')
 plt.title("Yield of Oranges (tons per hectare)");
```
![image](https://github.com/user-attachments/assets/81eaee90-fcf6-4e27-ba86-65ba369da278)
```
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 x=np.arange(0,10)
 y=np.arange(11,21)
 x
```
![image](https://github.com/user-attachments/assets/c798e09a-f993-4a9e-aa3f-87da616d61b9)
```
y
```
![image](https://github.com/user-attachments/assets/1e7b1268-6dbe-4879-b727-deba740b8c3c)
```
 plt.scatter(x,y,c='r')
 plt.xlabel('X-axis')
 plt.ylabel('Y-axis')
 plt.title('Graph in 2D')
 plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/77896d28-267f-4818-96e7-9037288f0907)
```
 y=x*x
 y
```
![image](https://github.com/user-attachments/assets/7ae22f0e-1e79-4955-963b-304657e83317)

```
 plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
 plt.xlabel('X axis')
 plt.ylabel('Y axis')
 plt.title('2d Diagram')
 plt.legend(['y-values']);
```
![image](https://github.com/user-attachments/assets/eb3e090e-e6b7-4549-8917-91e372fe6f7f)
```
 x=np.arange(0,4*np.pi,0.1)
 y=np.sin(x)
 plt.title("sine wave form")
 plt.plot(x,y)
 plt.show()
```
![image](https://github.com/user-attachments/assets/b83fab82-d1bc-4b3c-bdc1-97e28c4187b1)

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
![image](https://github.com/user-attachments/assets/e07e9f93-e4ee-4528-81a6-7092c027d9e7)

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
![image](https://github.com/user-attachments/assets/6b101825-0ad3-432a-91c7-f5a603ff3de9)

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
![image](https://github.com/user-attachments/assets/e97fa64b-161e-4619-8fb6-7ac43b0a9611)
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
![image](https://github.com/user-attachments/assets/f93beee1-0c13-4173-b010-2b387d286940)

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
![image](https://github.com/user-attachments/assets/718a2d8a-36a9-4fb1-adc8-f549fc32a916)
```
 import matplotlib.pyplot as plt
 import numpy as np
 np.random.seed(0)
 data=np.random.normal(loc=0,scale=1,size=100)
 data
```
![image](https://github.com/user-attachments/assets/621ea116-dca1-483a-822d-b7409af4ee7c)
```
 fig,ax=plt.subplots()
 ax.boxplot(data)
 ax.set_xlabel('Data')
 ax.set_ylabel('Values')
 ax.set_title('Box Plot')
```
![image](https://github.com/user-attachments/assets/2f472bd1-af43-49da-932f-c3a381b85c9a)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![image](https://github.com/user-attachments/assets/19cacd93-311a-4911-84b7-3bfbfd634dfe)
```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![image](https://github.com/user-attachments/assets/ec213035-9a30-41b7-a757-e7fed20333fb)

# Result:
 Thus, The implementation of data visualization using matplotlib has been successfully verified.
