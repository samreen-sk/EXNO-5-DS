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
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![Screenshot 2024-10-26 134043](https://github.com/user-attachments/assets/35f5e26c-875c-4441-9f8f-f26c09ee2234)

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
![Screenshot 2024-10-26 134837](https://github.com/user-attachments/assets/309fde07-c785-430a-aeef-12670a380a95)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![Screenshot 2024-10-26 134902](https://github.com/user-attachments/assets/2f8b9124-181b-495b-9489-412e03cce1d4)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```
![Screenshot 2024-10-26 134944](https://github.com/user-attachments/assets/e8e02cef-e8c2-4a31-827c-2d06b9450373)

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
![Screenshot 2024-10-26 135025](https://github.com/user-attachments/assets/fad46309-1f34-44aa-af4f-a7708f0cb716)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
```
![Screenshot 2024-10-26 135053](https://github.com/user-attachments/assets/dbcb9080-8c71-4f57-9897-bef8a82f983a)

```
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
```
![image](https://github.com/user-attachments/assets/8e00e9cd-c153-4bc4-9487-92c3275adfc6)

```
y
```
![image](https://github.com/user-attachments/assets/d1255c75-ea81-42cd-a73c-963bf4d8e4b4)

```
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![Screenshot 2024-10-26 135320](https://github.com/user-attachments/assets/11067581-325b-4226-9460-8f229ce36337)

```
y=x*x
y
```
![Screenshot 2024-10-26 135341](https://github.com/user-attachments/assets/f6327fb3-46f9-4676-9ffb-1a74f68aa539)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
```
![Screenshot 2024-10-26 135420](https://github.com/user-attachments/assets/f8283004-2b64-481d-8263-699927c7673a)

```
np.pi
```
![Screenshot 2024-10-26 135444](https://github.com/user-attachments/assets/06551a9b-c822-4f6d-a6df-fac6c4ab3d4e)

```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
```
![Screenshot 2024-10-26 135510](https://github.com/user-attachments/assets/339af2b5-b4c5-4968-9b9b-062f81c204fa)

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
![Screenshot 2024-10-26 135541](https://github.com/user-attachments/assets/1e182ec1-c017-4b81-8669-70c9078d5501)

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
![Screenshot 2024-10-26 135613](https://github.com/user-attachments/assets/6462e2e4-9b20-4190-b628-69bf82f9e78f)

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
![Screenshot 2024-10-26 135653](https://github.com/user-attachments/assets/4f11ea46-5dcc-4b73-bd06-e04d847c78f1)

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
![Screenshot 2024-10-26 135725](https://github.com/user-attachments/assets/b5c2cab8-c00e-4e36-9542-9dad654ac7c3)

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
![Screenshot 2024-10-26 135805](https://github.com/user-attachments/assets/118eed08-a2ab-4b27-a3ef-dedf89dc3ce6)

```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```
![Screenshot 2024-10-26 135841](https://github.com/user-attachments/assets/7f61de92-0c53-496f-86d6-38c9b5a4e417)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
```
![Screenshot 2024-10-26 135909](https://github.com/user-attachments/assets/5adb623b-9725-41bb-ab8b-c5fd9d9b3bee)

```
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![Screenshot 2024-10-26 135937](https://github.com/user-attachments/assets/959ed61c-3dda-403a-a8e1-5a0402f602b6)

```
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
```
![Screenshot 2024-10-26 140001](https://github.com/user-attachments/assets/3352f81f-60d7-4100-a410-2152cb15f151)

# Result:
 Include your result here
