## INDEX
[Program 01- Write a program to do linear search in python.](#Program-1)




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

