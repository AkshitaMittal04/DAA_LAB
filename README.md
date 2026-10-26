## INDEX
[Program 1- Write a program to show linear search in python.](#Program-1)
[Program 2- Write a program to show binary search in python.](#Program-2)




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

