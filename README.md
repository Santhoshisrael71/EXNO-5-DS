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
import numpy as np
import pandas as pd

x = [1, 2, 3, 4, 5]
y = [2, 4, 6, 8, 10]

plt.plot(x, y)
plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("Simple Line Graph")
plt.show()
```
<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/2c682298-c925-436a-b286-dfbcdefcde8b" />


```
x = [1, 2, 3, 4, 5]
y1 = [2, 4, 6, 8, 10]
y2 = [1, 3, 5, 7, 9]

plt.plot(x, y1, label="Line 1")
plt.plot(x, y2, label="Line 2")

plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("Two Lines Graph")
plt.legend()
plt.show()
```

<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/40f09b00-0704-476e-b7e1-a4240e5a2934" />


```
x = [1, 2, 3, 4, 5]
y = [2, 5, 3, 7, 9]

plt.plot(
    x,
    y,
    color='green',
    linestyle='dashed',
    linewidth=3,
    marker='o',
    markerfacecolor='blue',
    markersize=10
)

plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("Customized Plot")
plt.show()
```

<img width="554" height="453" alt="download" src="https://github.com/user-attachments/assets/e5c6296f-9ecc-4e70-8827-b92d3a51227a" />


```
x = [1, 2, 3, 4, 5]
y = [1, 4, 9, 16, 25]

plt.scatter(x, y, color='red', s=100)

plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("Scatter Plot")
plt.show()
```

<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/5c4b8d51-03f8-46e4-96b2-a4e782082058" />


```
x = np.arange(0, 10)
y = x * x

plt.plot(x, y, 'g*--', linewidth=2, markersize=10)

plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("2D Diagram")
plt.show()

```

<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/833439d3-adbf-402a-b753-ce6628bcf030" />


```
x = np.arange(0, 10)
y = x * x

plt.subplot(2, 2, 1)
plt.plot(x, y, 'r--')

plt.subplot(2, 2, 2)
plt.plot(x, y, 'g*-')

plt.subplot(2, 2, 3)
plt.plot(x, y, 'bo')

plt.subplot(2, 2, 4)
plt.plot(x, y, 'go')

plt.show()

```

<img width="543" height="413" alt="download" src="https://github.com/user-attachments/assets/76293207-a258-43d8-b96b-1b0f51309da1" />

```
x = np.arange(0, 4 * np.pi, 0.1)
y = np.sin(x)

plt.plot(x, y)

plt.title("Sine Wave Form")
plt.xlabel("X Axis")
plt.ylabel("Y Axis")

plt.show()
```

<img width="587" height="453" alt="download" src="https://github.com/user-attachments/assets/6458f269-aae3-46c2-8340-b52405c4df1b" />

```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [5, 7, 9, 11, 13]

plt.fill_between(x, y1, color='blue', alpha=0.5)
plt.fill_between(x, y2, color='green', alpha=0.5)

plt.title("Area Chart")
plt.show()
```

<img width="556" height="433" alt="download" src="https://github.com/user-attachments/assets/c88cda4c-c5d8-40fc-8b6a-de29f18679af" />


```
x = [1, 2, 3, 4, 5]
y1 = [10, 12, 14, 16, 18]
y2 = [2, 4, 6, 8, 10]
y3 = [5, 5, 5, 5, 5]

plt.stackplot(x, y1, y2, y3,
              labels=['Line1', 'Line2', 'Line3'])

plt.legend(loc='upper left')

plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.title("Stack Plot")

plt.show()
```

<img width="563" height="453" alt="download" src="https://github.com/user-attachments/assets/744e2de2-3b43-4f6f-aabf-c603cbb71913" />


```
names = ['A', 'B', 'C', 'D', 'E']
values = [5, 7, 3, 8, 6]

plt.bar(names, values, color='orange')

plt.xlabel("Names")
plt.ylabel("Values")
plt.title("Bar Graph")

plt.show()
```
<img width="554" height="453" alt="download" src="https://github.com/user-attachments/assets/d7737aa4-3769-4e96-aa6b-2167bace6586" />

```
plt.barh(names, values, color='green')

plt.xlabel("Values")
plt.ylabel("Names")
plt.title("Horizontal Bar Graph")

plt.show()
```

<img width="556" height="453" alt="download" src="https://github.com/user-attachments/assets/e2e24e18-6fec-4f5e-83ab-8c67c8f86212" />


```

data = [2,5,7,8,10,15,18,20,22,25,28,30,35,40]

plt.hist(data, bins=5, color='purple', alpha=0.7)

plt.xlabel("Value")
plt.ylabel("Frequency")
plt.title("Histogram")

plt.show()

```
<img width="567" height="453" alt="download" src="https://github.com/user-attachments/assets/803e9394-8c5d-4491-aade-719f784564bb" />


```
data = np.random.normal(0, 1, 100)

plt.boxplot(data)

plt.title("Box Plot")

plt.show()
```

<img width="546" height="433" alt="download" src="https://github.com/user-attachments/assets/8337536f-bc70-4a3b-90f3-304bbf4f7416" />

```
activities = ['Eat', 'Sleep', 'Work', 'Play']
slices = [3, 7, 8, 6]
colors = ['red', 'yellow', 'green', 'blue']

plt.pie(
    slices,
    labels=activities,
    colors=colors,
    autopct='%1.1f%%',
    shadow=True,
    startangle=90
)

plt.title("Pie Chart")

plt.show()
```
<img width="404" height="409" alt="download" src="https://github.com/user-attachments/assets/61111230-a76d-42c7-83fd-6d57784cb418" />


# Result:
 successfully Perform Data Visualization using matplot python library for the given datas.
