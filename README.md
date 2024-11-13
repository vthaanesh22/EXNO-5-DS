# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

## NAME:THAANESH
## REG NO:212223230228

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
~~~
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
~~~

![image](https://github.com/user-attachments/assets/651a2eac-48c0-4e06-bb85-18e1f0eeba5d)

~~~
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,3,5,1,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='red',markersize=10)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/a910ea69-99be-4b9f-9624-93b66b76d1e0)

~~~
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
~~~
![image](https://github.com/user-attachments/assets/575d1c35-40ce-442a-b74a-5f9e4b9625f2)

~~~
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
~~~
![image](https://github.com/user-attachments/assets/7622d784-b56e-4325-a66d-b5e8c1b885a4)

~~~
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
grapes=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, grapes)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields')
plt.legend(['Apples','grapes']);
~~~
![image](https://github.com/user-attachments/assets/cd71acdc-0e00-46d6-a7f4-cd5d7a3ba9bc)

~~~
plt.figure(figsize=(14,6))
plt.plot(years,grapes,marker='o')
plt.title("Yield of grapes (tons per hectare)");
~~~
![image](https://github.com/user-attachments/assets/faa43d64-8040-454b-b138-264969bac022)

~~~
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
~~~
![image](https://github.com/user-attachments/assets/26da30c7-6dab-4277-b37b-0a78bf414d9b)

~~~
y
~~~
![image](https://github.com/user-attachments/assets/7a23febd-2ab8-4267-838a-7490f4bda818)

~~~
plt.scatter(x,y,c='b')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
~~~
![image](https://github.com/user-attachments/assets/03634030-c7e7-496a-bc9f-c033885b689d)

~~~
y=x*x
y
~~~
![image](https://github.com/user-attachments/assets/23e04977-d5e0-437c-835c-b6743fdef05d)

~~~
np.pi
~~~
![image](https://github.com/user-attachments/assets/f7bcfe17-259d-4efc-92f9-865e2bf7c8d9)

~~~
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
~~~
![image](https://github.com/user-attachments/assets/b37ce8ed-92c0-4d98-8802-83cc2e984913)

~~~
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='red')
plt.fill_between(x,y2,color='green')
~~~
![image](https://github.com/user-attachments/assets/38a093e1-658f-4a87-ae52-c00186b4c317)

~~~
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
~~~
![image](https://github.com/user-attachments/assets/d0b05cbc-b0f6-4d5e-8a0e-8da7d37a9d64)

~~~
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
~~~
![image](https://github.com/user-attachments/assets/3274ebf9-c1a9-47ce-95f0-43f2d2947bcb)

~~~
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('Xaxis')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/1c18d9e6-7db9-4808-8353-f8a50c01628f)

~~~
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='lightblue',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/0490c327-d788-44f2-9e43-9ce8cb57e6d0)

~~~
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
~~~
![image](https://github.com/user-attachments/assets/152ca40d-4ee7-4c0c-b2df-33be074ee1bd)

~~~
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
~~~
![image](https://github.com/user-attachments/assets/10a1ff64-7b83-4e4d-ac31-0b09ee61eaf8)

~~~
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/1ae8eeb2-f4b4-4406-93e4-1ed201dc397e)

~~~
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
~~~
![image](https://github.com/user-attachments/assets/66453843-986a-43fa-97a8-3dedefe8f589)




















# Result:
 Thus, The implementation of data visualization using matplotlib has been successfully verified.
