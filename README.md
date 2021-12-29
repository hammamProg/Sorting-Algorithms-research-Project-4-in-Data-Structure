# Sorting Algorithms Project 4 in Data Structure

## 1) Strand Sort

it's a sorting algorithms based on recursion, this algorithm sorts items of a list in an increasing order.

### Time Complexity:
- In the worst case(where the list is in reverse order) it takes `O(n^2)`.
- In the best case ( where the list is already sorted) it takes `O(n)`

### How its work(algorithm): 

	1- At first take the first element in the list into a sub list, and remove it from the main list.
  
	2- Then compare the last element in the sub list (supose it = X) to each subsequent element in main list(supose it = Y), 
	if Y is greater than X :add Y to the last of sub_list and remove Y from the main list,
	continue until the end of the main_list.
  
	3- After that, merge the existing sub_list to the sorted_list(which is empty at first time),
	and remove all elements in sub_list.
  
	4- Repeat this until the main list becoming empty

### Animation:

![strand_sort_gif](/Media/StrandSort.gif)

### Implementation:


  [Strand Sort Code](/Code/app.py)
  #### Result
  ![strand_sort_test](/Media/Strand_sort_test.PNG)



## 2) Timsort

it's a combination of two algorithms ( insertion and merge ) , and it was implemented by Tim Peters in 2002 for use in the Python programming language


### Time Complexity:
- In the worst case(where the list is in reverse order) it takes `O(nlogn)`.
- In average case it takes `O(nlogn)`
- In the best case ( where the list is already sorted) it takes `O(n)`

### How its work(algorithm): 

	1- Divide the array into the number of block known as `run`
  
	2- the size of run could be considered either 32 or 64
  
	3- By the insertion(sort algorithm), sort all individual elements of every run -> one by one
  
	4- By merge function in the merge sort, merge the sorted runs -> one by one
	
	5- After each iteration double the size of merged sub-arrays


### Implementation:


  [Timsort Code](/Code/Timsort.pyy)
  #### Result
  ![Temsort_image](/Media/timsort.png)

## 3) Cycle Sort



### Time Complexity:
- In the worst case(where the list is in reverse order) it takes `O(n^2)`.
- In average case it takes `O(n^2)`
- In the best case ( where the list is already sorted) it takes `O(n^2)`

### How its work(algorithm): 

	1- Choose the first element(suppose it = X) of an array.
  
	2- Compare it with all elements in this array.
  
	3- Count the number of element greater than this(X) and the count represent the position of X in the array.
  
	4- Switch X with the element in its position.
	
	5- if the first element is in the right position move to next index.
	
	6- repeat this steps until the array is sorted.
	
	
### Implementation:


  [Timsort Code](/Code/Timsort.pyy)
  #### Result
  ![Temsort_image](/Media/timsort.png)




### References

 1) StrandSort:
	- https://www.pythonpool.com/python-strand-sort
	- https://en.wikipedia.org/wiki/Strand_sort
 2) Temsort:
 
     	- https://en.wikipedia.org/wiki/Timsort
     	
     	- https://hackernoon.com/timsort-the-fastest-sorting-algorithm-youve-never-heard-of-36b28417f399
     	
     	- https://www.geeksforgeeks.org/timsort/	
     	
     	- https://www.youtube.com/watch?v=9kFHVe5MT6o
     	- 
     	- https://www.javatpoint.com/tim-sort
 

   
   
   Choose algorithms by this article on geeksforgeeks:
	https://www.geeksforgeeks.org/sorting-algorithms/


