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
 Include the necessary coding and corresponding screenshots
 ```
import matplotlib.pyplot as plt
x1=[1,2,3]
y1=[2,4,1]
plt.plot(x1,y1,label="line 1")
x2=[1,2,3]
y2=[4,1,3]
plt.plot(x2,y2,label="line 2")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph')
plt.legend()
```
![Screenshot 2024-10-22 113932](https://github.com/user-attachments/assets/b1c1ad7a-69e6-4aeb-925f-c796a7bdde91)
```
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='red',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='yellow',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
```
![Screenshot 2024-10-22 114017](https://github.com/user-attachments/assets/ed26ef22-0f7c-40a0-b449-610673bb8f4d)
```
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.92,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896]
plt.xlabel('Year')
plt.ylabel('Yield')
plt.plot(years,apples,label='Apples')
plt.plot(years,oranges,label='Oranges')
plt.legend()
```
![Screenshot 2024-10-22 114041](https://github.com/user-attachments/assets/f96826bb-a425-4832-bd39-6413e08ba125)
```
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="red")
```
![Screenshot 2024-10-22 114108](https://github.com/user-attachments/assets/50cc863c-17f5-4c8a-a476-3ebb352ce368)
```
x_values=[1,2,3,4,5,6,7,8,9,10]
y_values=[2,4,5,7,6,8,9,11,12,12]
plt.scatter(x_values,y_values,label="square" ,s=30,color="blue",marker="*")
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("My scatter plot")
plt.legend()
```
![Screenshot 2024-10-22 114141](https://github.com/user-attachments/assets/3081f763-c738-4349-8eed-6bd57eb81e32)
```
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
print(x)
print(y)
```
![Screenshot 2024-10-22 114211](https://github.com/user-attachments/assets/e2fcd5ee-f1d2-4c1b-a337-4844b108628a)
```
plt.scatter(x,y,c='b')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Graph in 2D')
plt.savefig('scatter.jpeg')
```
![Screenshot 2024-10-22 114235](https://github.com/user-attachments/assets/4f3ef9d5-202a-4cea-a0d5-bd1959850d75)
```
x=np.arange(0,10)
y=x*x
y
```
![Screenshot 2024-10-22 114302](https://github.com/user-attachments/assets/fe51f8d1-2484-4038-9aad-6793727b3f97)
```
plt.plot(x,y,'r*',linestyle='dashed',linewidth=5,markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('2D diagram')
```
![Screenshot 2024-10-22 114309](https://github.com/user-attachments/assets/4670583e-76a9-440e-be8c-f09031cb16e6)
```
np.pi
```
![Screenshot 2024-10-22 114412](https://github.com/user-attachments/assets/934e710a-0306-4234-a547-77ad18c235e6)
```
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title('Sine wave')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.plot(x,y)
```
![Screenshot 2024-10-22 114442](https://github.com/user-attachments/assets/892bb49d-b364-4a81-9291-3811761fa4ba)
```
plt.subplot(2,2,1)
plt.plot(x,y,'b--')
plt.subplot(2,2,2)
plt.plot(x,y,'r*--')
plt.subplot(2,2,3)
plt.plot(x,y,'bo')
plt.subplot(2,2,4)
plt.plot(x,y,'go')
```
![Screenshot 2024-10-22 114509](https://github.com/user-attachments/assets/9208fbc8-a186-4281-982a-cb878d3d708e)
```
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='red')
plt.fill_between(x,y2,color='blue')
plt.plot(x,y1,color='green')
plt.plot(x,y2,color='yellow')
plt.legend(['y1','y2'])
plt.show()
```
![Screenshot 2024-10-22 114536](https://github.com/user-attachments/assets/24637539-cdc1-4d0b-a754-d55bf91f889b)
```
plt.stackplot(x,y1,y2,y3,labels=['Line1','Line2','Line3'])
plt.legend(loc='upper left')
plt.title('Stacked Line Chart')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![Screenshot 2024-10-22 114601](https://github.com/user-attachments/assets/eaef89cd-f62e-4376-acca-68a304a2b33d)
```
val=[5,6,3,7,2]
name=["A","B","C","D","E"]
plt.bar(name,val,color='pink')
plt.show()
```
![Screenshot 2024-10-22 114624](https://github.com/user-attachments/assets/63749614-1b19-480e-a710-eab900b296a9)
```
h=[10,24,36,40,100]
name=['one','two','three','four','five']
c1=['r','g']
c2=['b','y']
plt.bar(name,h,color=c1,width=0.5)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Bar graph')
plt.show()
```
![Screenshot 2024-10-22 114649](https://github.com/user-attachments/assets/806fb9a1-ee70-4470-b5a5-458952d18e1e)
```
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='y')
plt.bar(x2,y2,color='pink')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Bar graph')
plt.show()
```
![Screenshot 2024-10-22 114752](https://github.com/user-attachments/assets/31ca1a59-932b-4144-8123-8b1e978dd24f)
```
ages=[2,5,70,40,30,45,43,44,40,60,7,13,56,19,90,77,33,23,20,40]
range=(0,100)
bins=15
plt.hist(ages,bins,range,color='black',histtype='step',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no.of.people')
plt.title('Histogram')
plt.show()
```
![Screenshot 2024-10-22 114816](https://github.com/user-attachments/assets/057c9533-691c-41c3-abf2-635e6b649ab1)
```
x=[2,1,6,4,2,4,8,9,4,2,4,10,6,4,5,7,7,7,2,5,8,9,0,6,8,9,3]
plt.hist(x,bins=10,color='pink',alpha=1)
plt.show()
```
![Screenshot 2024-10-22 114846](https://github.com/user-attachments/assets/dae6baf6-9eab-4b2a-a649-5c665bdbac18)
```
np.random.seed(0)
d=np.random.normal(loc=0,scale=1,size=100)
d
```
![Screenshot 2024-10-22 114914](https://github.com/user-attachments/assets/9414cc16-71a4-41fb-a012-cc8ca8fc1c1c)
```
f,ax=plt.subplots()
ax.boxplot(d)
ax.set_xlabel('data')
ax.set_ylabel('values')
ax.set_title('Box plot')
plt.show()
```
![Screenshot 2024-10-22 114938](https://github.com/user-attachments/assets/d83420f8-b646-4129-9b8f-53942d6a0dae)
```
act=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['grey','red','pink','blue']
plt.pie(slices,labels=act,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),autopct='%1.1f%%')
plt.legend()
plt.show()
```
![Screenshot 2024-10-22 115002](https://github.com/user-attachments/assets/3848fe54-4f4c-4080-ab31-cec67552f832)
```
labels='Py','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.6)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
```
![Screenshot 2024-10-22 115026](https://github.com/user-attachments/assets/b7a1f721-2fd2-4307-bff9-d8c05736084c)

# Result:
 Thus the code for data visualization executed successfully.
