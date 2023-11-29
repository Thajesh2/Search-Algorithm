# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
Program for linear search method to match the item in a list
Developed by: Thajesh k
RegisterNumber: 23004042

def linearSearch(array,n,k):
    for i in range(0,n):
      if (array[i]==k):
          return i
    return -1 
          
array=eval(input())
array=sorted(array)
n=len(array)
k=eval(input())
res = linearSearch(array,n,k)
if(res==-1):
   print(array)
   print("Element not found")
else:
    print(array)
    print("Element found at index: ",res)

```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by: Thajesh k
RegisterNumber: 23004042


def linearSearch(array,n,k):
    for i in range(0,n):
        if (array[i]==k):
          return i
    return -1 
          
array=eval(input())
array=sorted(array)
n=len(array)
k=eval(input())
res = linearSearch(array,n,k)
if(res==-1):
   print(array)
   print("Element not found")
else:
    print(array)
    print("Element found at index: ",res)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
Program to find the element in a list using Binary Search (recursive Method).
Developed by: Thajesh k
RegisterNumber: 23004042

def BinarySearch(arr,low,high,x):
    if high>=low:
        mid= (high + low)//2
        if arr[mid]==x:
            return mid
        elif arr[mid]>x:
            return BinarySearch(arr,low,mid-1,x)
        else:
            return BinarySearch(arr,mid+1,high,x)
    else:
            return -1
            
            
            
arr = eval(input())
arr=sorted(arr)
x=eval(input())
result=BinarySearch(arr,0,len(arr)-1,x)
if result!=-1:
    print(arr)
    print("Element found at index: ",str(result))
else:
    print(arr)
    print("Element not found")




```
## Output
![image](https://github.com/Thajesh2/Search-Algorithm/assets/139841959/917800d0-ff1c-4db7-ba1c-43eb4302aca5)


![image](https://github.com/Thajesh2/Search-Algorithm/assets/139841959/946e4f11-c475-4fb0-8ae8-5e440c7759f9)


![image](https://github.com/Thajesh2/Search-Algorithm/assets/139841959/52c43d02-4917-4fce-a42b-fced792a8ac7)






## Result
Thus the linear search and binary search algorithm is implemented using python programming.
