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
# Developed By   : SANJAY M
# Register No    : 212223230187


def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)


```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
# Developed By   : SANJAY M
# Register No    : 212223230187


def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)




```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
# Developed By   : SANJAY M
# Register No    : 212223230187

def binarySearchIter(array, k, low, high):
    while low<=high:
        mid=low+(high-low)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
array = eval(input())
array.sort()
k = eval(input()) 
print(array)
res=binarySearchIter(array,k,0,len(array)-1)
if res==-1:
    print("Element not found")
else:
    print("Element found at index: ",res)




```
## Sample Input and Output:
![Screenshot 2024-04-02 174310](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/1be482d8-13a0-467d-8758-8dd2be1684c6)
![Screenshot 2024-04-02 174319](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/4486623a-6ce3-42d3-9873-8729a5f8757e)
![Screenshot 2024-04-02 174338](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/2a6ea525-8231-4fdf-862f-41b6ea1c0803)
![Screenshot 2024-04-02 174347](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/538eb3e7-7745-4a34-b796-70a64675cf0f)
![Screenshot 2024-04-02 174424](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/035b798a-c602-4977-b916-0fd3470052fc)
![Screenshot 2024-04-02 174433](https://github.com/sanjayofficial2005/Search-Algorithms/assets/148048602/00794e67-cd00-477c-a0dc-6eb280dcd462)








## Result
Thus the linear search and binary search algorithm is implemented using python programming.
