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
x=[2018, 2019, 2020, 2021, 2022]
y=[15000, 20000, 25000, 30000, 35000]
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('xaxis')
plt.ylabel('yaxis')
plt.title('2D Diagram')
plt.show()
```

<img width="1173" height="897" alt="image" src="https://github.com/user-attachments/assets/d55747f0-cedd-4ce0-b6be-a43a31bea327" />


```
plt.subplot(2,2,1)
plt.plot(x,y,'r--')
plt.subplot(2,2,2)
plt.plot(x,y,'g--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
<img width="1176" height="879" alt="image" src="https://github.com/user-attachments/assets/0ec16550-f75b-4c3a-9774-ac13e89dc1ac" />




```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine waveform")
plt.plot(x,y)
plt.show()
```
<img width="1132" height="867" alt="image" src="https://github.com/user-attachments/assets/b81f1d80-c599-48d5-8e99-68ee985e77fd" />




```
x=[2,8,10]
y=[11,16,9]
x1=[3,9,11]
y1=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x1,y1,color='g')
plt.title("Bar Garph")
plt.xlabel('xaxis')
plt.ylabel('yaxis')
plt.show()
```
<img width="1127" height="922" alt="image" src="https://github.com/user-attachments/assets/8aa375f7-0848-49b6-b72b-6cb2c5214b9c" />



```
x=[1,2,3]
y=[7,3,9]
plt.plot(x,y,color='g')
plt.title("Line Garph")
plt.xlabel('xaxis')
plt.ylabel('yaxis')
plt.show()
```

<img width="1109" height="898" alt="image" src="https://github.com/user-attachments/assets/897237a1-7936-43e6-8a79-752300dcee7b" />




```
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label='line1')
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label='line2')
plt.title("Multiline Graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="1127" height="910" alt="image" src="https://github.com/user-attachments/assets/015633a9-21e5-414c-9ae2-72f8fc507453" />


```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='red',markersize=12,label='spices')
plt.ylim(1,8)
plt.xlim(1,8)
plt.title("Line Graph")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="1107" height="914" alt="image" src="https://github.com/user-attachments/assets/ff1dedba-15ac-4928-aee4-89e2974bbf50" />




```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples,linestyle='dashed',linewidth=3,marker='*',markersize=12,color='g')
plt.show()
```

<img width="1152" height="833" alt="image" src="https://github.com/user-attachments/assets/6b6567f8-a953-4790-98d8-cfadb8e9071b" />



```
oranges=[2,4,6,8,12,45,50]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022,2023,2024,2025]
plt.plot(years, apples, marker='o')
plt.plot(years, oranges, marker='*')
plt.title("crop yields in kanto")
plt.xlabel('year')
plt.ylabel('Yield(tons per hectare)')
plt.legend(['apples', 'oranges'])
plt.show()
```

<img width="1124" height="914" alt="image" src="https://github.com/user-attachments/assets/8b09b473-3d13-42d0-b389-e0916c4d24fc" />



```
oranges=[2,4,6,8,12,45,50]
apples=[2,4,5,6,8,23,37]
years=[2019,2020,2021,2022,2023,2024,2025]
plt.bar(oranges, apples)
plt.plot(years, apples, label='apples', marker='o')
plt.plot(years, oranges, label='oranges', marker='*')
plt.title("Fruit Sales")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="1119" height="898" alt="image" src="https://github.com/user-attachments/assets/273e49f7-ccb6-4850-a75a-2c9a4e80409d" />




```
plt.figure(figsize=(12,6))
plt.plot(years, oranges, marker='o', label='oranges')
plt.title("Yield of oranges (tons per hectare)")
plt.legend()
```

<img width="1948" height="1097" alt="image" src="https://github.com/user-attachments/assets/70f2865d-6210-4b86-824a-fca5dfb626d2" />




```
print("Scatter plot is:")
x=[1,2,3,4,5,6,7,8,9,10]
y=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x,y, label='star', color='green', marker='*',s=30)
plt.title("my scatterplot!")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.legend()
plt.show()
```

<img width="1122" height="953" alt="image" src="https://github.com/user-attachments/assets/5f510d89-9c56-4ddf-bfe3-c87a279c1b01" />



```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='green', label='y1')
plt.fill_between(x,y2,color='blue', label='y2')
plt.fill_between(x,y3,color='red', label='y3')
plt.title("fill between is")
plt.legend()
plt.show()
```

<img width="1105" height="866" alt="image" src="https://github.com/user-attachments/assets/6040c7b8-50d6-4ce9-b91c-607a357043d4" />




```
plt.stackplot(x,y1, y2,y3, labels=['line1', 'line2', 'line3'])
plt.legend(loc='upper left')
plt.title("Stacked line chart")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```

<img width="1121" height="908" alt="image" src="https://github.com/user-attachments/assets/3bda4d8c-ed93-4a8b-bce2-880d0e8d2886" />




```
from scipy.interpolate import make_interp_spline
x=np.array([1,2,3,4,5,6,7,8,9,10])
y=np.array([2,4,5,7,8,9,10,11,12,13])
spl=make_interp_spline(x,y)
x_smooth=np.linspace(x.min(),x.max(),100)
y_smooth=spl(x_smooth)
plt.plot(x,y,'o', label='data')
plt.plot(x_smooth,y_smooth,'-', label='spine')
plt.legend()
plt.show()
```

<img width="1064" height="832" alt="image" src="https://github.com/user-attachments/assets/49802388-8ac2-4b4d-9f22-1021558dcbdf" />




```
values=[5,6,7,3,2]
names=['A','B','C','D','E']
plt.bar(names,values,color='green')
plt.show()
```
<img width="1065" height="819" alt="image" src="https://github.com/user-attachments/assets/66b4bc59-a905-4972-8328-62f07a374064" />






```
ages=[2,5,70,40,45,50,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range1=(0,100)
bins=10
plt.hist(ages, bins, color='green', histtype='bar', rwidth=0.8)
plt.xlabel('ages')
plt.ylabel('no.of people')
plt.title('my histogram')
plt.show()
```

<img width="1099" height="906" alt="image" src="https://github.com/user-attachments/assets/a2ca8392-9fbb-4b76-8790-2107f2e5b551" />




```
x=[2,1,6,2,4,8,9,4,2,4,10,6,4,5,7,7,3,2,7,5,3,5,9,2,1]
plt.hist(x,bins=10,color='green', alpha=0.5)
plt.show()
```

<img width="1077" height="840" alt="image" src="https://github.com/user-attachments/assets/f53c503a-626e-4aab-a18d-d3c6de8e368c" />




```
np.random.seed(0)
data=np.random.normal(loc=0, scale=1, size=100)
data
```

<img width="1199" height="717" alt="image" src="https://github.com/user-attachments/assets/a7c7cfff-2a20-41e3-a25f-7b4d06677f3e" />




```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('x-axis')
ax.set_ylabel('y-axis')
ax.set_title('box plot')
```

<img width="1132" height="952" alt="image" src="https://github.com/user-attachments/assets/e2292769-2603-429b-9535-3a8b3dc1adf7" />






```
activities=['eat', 'sleep', 'work', 'play']
slices=[3,7,8,6,]
colors=['r','y','g','b']
plt.pie(slices, labels=activities, colors=colors, startangle=90, shadow=True, explode=(0,0,0.1,0), radius=1.2, autopct="X1.1")
plt.legend()
plt.show()
```
<img width="1495" height="1376" alt="image" src="https://github.com/user-attachments/assets/dd76d252-a612-4280-a5f9-c5ff038f044c" />

<img width="866" height="821" alt="image" src="https://github.com/user-attachments/assets/1addfd55-dda1-4b55-83ca-58e560dbdb7e" />



```
labels='python', 'C+','ruby','java'
sizes=[215,130,245,210]
colors=['gold', 'yellowgreen','lightcoral', 'lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes, explode=explode, colors=colors, labels=labels, autopct='%1.1f%%', shadow=True)
plt.axis('equal')
plt.show()
```

<img width="1021" height="771" alt="image" src="https://github.com/user-attachments/assets/dcc4eb4c-a55e-460c-8da2-f9f67b09cbbd" />






# Result:
Thus the program is executed successfully.

