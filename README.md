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
Developed By: Krishna Prasad.S
Register No: 212223231018
```

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.plot(x_values,y_values)
plt.show()
```
![image](https://github.com/user-attachments/assets/f921983f-faf9-4baf-8c16-466cf71fa97f)

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
![image](https://github.com/user-attachments/assets/24211c47-2b5f-48d0-92e0-b17fa2a3db45)

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
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
```
![Screenshot 2024-10-19 194514](https://github.com/user-attachments/assets/3009d21f-d0e3-4c31-9b79-f2a26573ff01)

```
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.ylim(1,8)
plt.xlim(1,8)

plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')

plt.show()
```
![Screenshot 2024-10-19 194554](https://github.com/user-attachments/assets/1a9f620c-f2b5-4e85-9442-18ff7fb607f9)

```
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
```
![Screenshot 2024-10-19 194634](https://github.com/user-attachments/assets/84e18b7e-45c3-471b-8112-1360b18662a3)

```
years=[2010,2011,2012,2013,2014,2015]
yeild_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yeild_apples)
```
![Screenshot 2024-10-19 194725](https://github.com/user-attachments/assets/9f9e07fe-9a4d-40a1-abbf-691d8c503d34)

```
plt.plot(years, yield_apples)
plt.xlabel('Year')
plt.ylabel('Year (tons per hectare)')
```
![Screenshot 2024-10-19 194939](https://github.com/user-attachments/assets/5d468789-9dc9-441a-b66d-c961a84e4de1)

```
years=range(2000,2012)
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yeild of Oranges (tons per hectare)");
```
![Screenshot 2024-10-19 195135](https://github.com/user-attachments/assets/0c171f19-4e03-46be-be22-9476d465b0b4)

```
years=range(2000,2012)
apples= [0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.962,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896,]
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)');
```
![Screenshot 2024-10-19 195247](https://github.com/user-attachments/assets/d1b2b554-0fda-4c2f-b72b-aec953ccf25e)

```
plt.plot(years,apples)
plt.plot(years,oranges)
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```
![Screenshot 2024-10-19 195320](https://github.com/user-attachments/assets/b69e54c8-695e-4cc7-a8c1-8e0eec8011d6)

```
plt.plot(years,apples,marker='o')
plt.plot(years,oranges,marker='x')
plt.xlabel('Year')
plt.ylabel('Yeild(tons per hectare)')
plt.title("Crop Yeilds in Kanto")
plt.legend(['Apples','Oranges']);
```
![Screenshot 2024-10-19 195404](https://github.com/user-attachments/assets/b20a996d-7adc-4997-b193-bcff58d49b10)

```
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color="blue")
plt.fill_between(x,y2,color="green")
plt.plot(x,y1,color="red")
plt.plot(x,y2,color="black")
plt.legend(['y1','y2'])
plt.show()
```
![Screenshot 2024-10-19 195812](https://github.com/user-attachments/assets/b7dd45c9-c794-460d-bb5b-8db73b26c1ba)

```
import numpy as np
import matplotlib.pyplot as plt
from scipy.interpolate import make_interp_spline
x = np.array([1, 2, 3, 4, 5, 6, 7, 8, 9, 10])
y = np.array([2, 4, 5, 7, 8, 8, 9, 10, 11, 12])
spl = make_interp_spline(x, y)
x_smooth = np.linspace(x.min(), x.max(), 100)
y_smooth = spl(x_smooth)
plt.plot(x, y, 'o', label='data')
plt.plot(x_smooth, y_smooth, '-', label='spline')
plt.legend()
plt.show()
```
![Screenshot 2024-10-19 200239](https://github.com/user-attachments/assets/9756c81a-ea68-4668-b0d4-3b60636096b0)

```
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No.of people')
plt.title('My histogram')
plt.show()
```
![Screenshot 2024-10-19 200335](https://github.com/user-attachments/assets/7ff482ac-3765-4988-bd4c-ac123da78f28)

```
import matplotlib.pyplot as plt
values = [5,6,3,7,2]
names = ["A", "B", "C", "D", "E"]
plt.barh (names, values, color="yellowgreen")
plt.show()
```
![Screenshot 2024-10-19 200531](https://github.com/user-attachments/assets/0494d001-4304-4d3f-a9ce-5e2e85a0c0ce)

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
![Screenshot 2024-10-19 200611](https://github.com/user-attachments/assets/05921ef8-bce0-4820-b592-47c97262212e)

```
import matplotlib.pyplot as plt
x_values=[0,1,2,3,4,5]
y_values=[0,1,4,9,16,25]
plt.scatter(x_values,y_values,s=30,color="blue")
plt.show()
```
![Screenshot 2024-10-19 200652](https://github.com/user-attachments/assets/8cd4f51d-cd00-4213-a11f-febd3ffd8a9e)

```
import matplotlib.pyplot as plt
x = [1,2,3,4,5,6,7,8,9,10]
y = [2,4,5,7,6,8,9,11,12,12]
plt.scatter (x, y, label= "stars", color="green", marker="*", s=30)
plt.xlabel('x axis')
plt.ylabel('y - axis')
plt.title('My scatter plot!')
plt.legend()
plt.show()
```
![Screenshot 2024-10-19 200839](https://github.com/user-attachments/assets/f290728c-e044-475a-92b1-553bbec39e7c)

```

```
# Result:
 Include your result here
