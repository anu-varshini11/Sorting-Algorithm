# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
i)	#Selection Sort
```PYTHON
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: M B ANU VARSHINI
RegisterNumber: 23008712 
'''
def selection_sort(nums):
    for i in range(len(nums)):
        low=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[low]:
                low=j
        nums[i],nums[low]=nums[low],nums[i]
    print(nums)
list_of_nums = eval(input())
selection_sort(list_of_nums)
```
ii)	#Insertion Sort
```PYTHON
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: M B ANU VARSHINI
RegisterNumber: 23008712
'''
def insertion_sort(nums):
    for i in range(len(nums)):
        insert=nums[i]
        j=i-1
        while j>=0 and nums[j]>insert:
            nums[j+1]=nums[j]
            j=j-1
        nums[j+1]=insert
    print(nums)
list_of_nums = eval(input())
insertion_sort(list_of_nums)
```

## Output:
![sort](https://github.com/anu-varshini11/Sorting-Algorithm/assets/138969827/e8c9a6b4-c10d-4dfa-be98-f7dcfdf50a4a)
![sort2](https://github.com/anu-varshini11/Sorting-Algorithm/assets/138969827/a0a73d66-3ee0-471e-9190-5d829c4547e4)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
