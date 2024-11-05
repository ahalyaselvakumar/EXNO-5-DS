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
import numpy as np
import pandas as pd
```

```
x=np.arange(0,10)
y=np.arange(11,21)
x
y
``` 

![image](https://github.com/user-attachments/assets/0f76ef9b-5c7e-4e18-aaf5-2cf7695e89ab)

```
x=np.arange(40,50)
y=np.arange(50,60)
x
y
```

![image](https://github.com/user-attachments/assets/888c5056-e420-47ea-9ba4-50cf75f9fc42)

```
#Scatterplot
plt.scatter(x,y,c='r')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
```
![image](https://github.com/user-attachments/assets/e0cf5af9-3576-41b2-877d-336cb6ee141f)

```
y=x*x
y
```
![image](https://github.com/user-attachments/assets/18af4b9a-4973-458f-a05e-154ad0485fd9)

```
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2D Diagram')
```

![image](https://github.com/user-attachments/assets/efee12cb-9cc4-4f23-83c8-2d1b2476b34e)

```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![image](https://github.com/user-attachments/assets/93f4c26c-6096-4113-af3d-4fc96f4ed1bc)

```
# Compute the x and y coordinates for points on a
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")

#Plot the points using matplotlib
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/3a5225f8-c922-4ca2-a619-af521359ff92)

```
#BAR Chart
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.show()
```
![image](https://github.com/user-attachments/assets/37b2671b-8e80-4d84-b0ea-211cd6ea97f7)

```
x=np.arange(1,11)
y=3*x+5
plt.title("Matplotlib demo")
plt.xlabel("x axis caption")
plt.ylabel("y axis caption")
plt.plot(x,y)
plt.show()
```
![image](https://github.com/user-attachments/assets/2296dbcb-4228-4826-a63d-8173c82e86f9)

```
x=np.arange(0,5 *np.pi,0.1)
y_sin=np.sin(x)
y_cos=np.cos(x)
plt.subplot(2,1,1)
plt.plot(x,y_sin,'r--')
plt.title('Sine')
plt.subplot(2,1,2)
plt.plot(x,y_cos,'g--')
plt.title('Cosine')
plt.show()
```
![image](https://github.com/user-attachments/assets/a9ea1f15-672c-4410-90cb-ed19c3bc1a39)

```
a=np.array([22,87,5,43,56,73,55,54,11,20,51,5,79,31,27])
plt.hist(a,color='g')
plt.title("histogram")
plt.show()
```
![image](https://github.com/user-attachments/assets/2b6ced6c-2dab-4539-ae43-77997bd6e97f)

```
labels=['A','B','C']
values=[1,4,2]
plt.figure(figsize=(5,3),dpi=100)
bars=plt.bar(labels,values,color='green')
patterns=['-','*','+']
for bar in bars:
  bar.set_hatch(patterns.pop(0))
plt.savefig('barchat.png',dpi=100)
plt.show()
```

![image](https://github.com/user-attachments/assets/071585e2-7712-4e36-b02e-5138f0fb8074)

```
import matplotlib.pyplot as plt
x_values = [0,1,2,3,4,5]
y_values = [0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/user-attachments/assets/cbe05c0b-1243-4a99-9656-1c8d38ae88a2)

```
import matplotlib.pyplot as plt
x=[1,2,3]
y=[2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph!')
plt.show()
```
![image](https://github.com/user-attachments/assets/5475b35a-b25b-40b5-ad10-1b6584263788)

```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/509aa10e-e7c0-490b-abe3-825c4fe54b5b)

```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6]
y = [2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,
         marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customization')
plt.show()
```

![image](https://github.com/user-attachments/assets/31ee8ae6-bbc1-4aa8-b84f-bd3335d580b9)

```
yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```

![image](https://github.com/user-attachments/assets/282b94c6-5ec5-469d-929d-ff6ffc6fbb7b)

```
years=[2010,2011,2012,2013,2014,2015]
yield_apples = [0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
```

![image](https://github.com/user-attachments/assets/b3b173e3-86dd-44dc-8a6d-32c3f465636e)

```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.900,0.907,0.904,0.901,0.898,0.9,0.896]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel("year")
plt.ylabel("Yield(toes per hectare)");
```
![image](https://github.com/user-attachments/assets/3578e728-f742-4dd7-88a9-ec2152b65611)

```
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of oranges (toes per hectare)");
```
![image](https://github.com/user-attachments/assets/dfdaf603-54cb-47f2-b4fe-183f6cf3009b)

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges'])
```

![image](https://github.com/user-attachments/assets/1d78a880-91ee-453b-8878-01a8547886e1)

```
import matplotlib.pyplot as plt
x_values = [1,2,3,4,5,6,7,8,9,10]
y_values = [2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y,label="stars",color="blue",marker="*",s=30)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("My scatter plot!")
plt.legend()
plt.show()
```
![image](https://github.com/user-attachments/assets/4c44812e-edd7-4f61-ac8c-de045e0763b2)

```
AREA CHART
```
```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="blue")
plt.fill_between(x,y2,color="green")
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
```
![image](https://github.com/user-attachments/assets/da507cf0-ad15-4aea-8536-7715cc7f6dad)

```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2','Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.show()
```

![image](https://github.com/user-attachments/assets/ffccc359-cc5d-4c76-907d-05a2feddb0dc)

```
SPLINE CHART
```
```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x = np.array([1,2,3,4,5,6,7,8,9,10])
y = np.array([2,4,5,6,7,8,8,10,11,12])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o',label='data')
plt.plot(x_smooth,y_smooth,'-',label='spline')
plt.legend()
plt.show()
```

![image](https://github.com/user-attachments/assets/40042769-eaea-4f27-8f6e-9ffd8dacd69c)

# Result:
 Thus the program to Perform Data Visualization using matplot python library for the given datas is been implemented.
