## INDEX
[Program 1- Write a program to show linear search in python.](#Program-1)

[Program 2- Write a program to show binary search in python.](#Program-2)

[Program 10- Write a Python program to plot a line graph using the given x and y values.](Program-10)

[Program 11- Write a Python program to plot multiple graphs for log(n), n, n log(n), and n².](Program-11)



## Program-1
```
def linear_search(arr, target):
    for i in range(len(arr)):
        if arr[i] == target:
            return i
    return -1


numbers = [10, 20, 30, 40, 50]
target = 30

result = linear_search(numbers, target)

if result != -1:
    print("Element found at index", result)
else:
    print("Element not found")
```
##Program-2
```
def binary_search(arr,key):
    low=0
    high=len(arr)-1
    while low<=high:
        mid=(low+high)//2
        
        if arr[mid]==key:
            return mid
        elif arr[mid]<key:
            low=mid+1
        else:
            high=mid-1
    return -1
arr=[10,20,30,40,50]
key=int(input("Enter element to search"))
result=binary_search(arr,key)
if result!=-1:
    print("Element found at index",result)
else:
    print("Element not found")
```
##Program-10
```
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 15, 30, 25]

plt.plot(x, y)
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.title("Simple Line Graph")
plt.show()
```
<img width="801" height="601" alt="image" src="https://github.com/user-attachments/assets/b9682426-1f07-4d31-addc-70744d2f0ee3" />

##Program-11
```
import matplotlib.pyplot as plt
import math

x = [1, 2, 3, 4, 5]

y1 = [math.log(i) for i in x]
y2 = [i for i in x]
y3 = [i * math.log(i) for i in x]
y4 = [i * i for i in x]

plt.plot(x, y1, marker='o')
plt.plot(x, y2, marker='o')
plt.plot(x, y3, marker='o')
plt.plot(x, y4, marker='o')

plt.title("Line Graph")
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.grid(True)
plt.show()
```
<img width="796" height="607" alt="image" src="https://github.com/user-attachments/assets/1c9d77c0-637f-4825-b582-1e959835cb53" />


