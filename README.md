# Sorting Algorithms Project 4 in Data Structure

## 1) Strand Sort

it's a sorting algorithms based on recursion, this algorithm sorts items of a list in an increasing order.

Time Complexity:
- In the worst case(where the list is in reverse order) it takes `O(n^2)`.
- In the best case ( where the list is already sorted) it takes `O(n)`

Note:  


how its work(algorithm): 

	1- At first take the first element in the list into a sub list, and remove it from the main list.
  
	2- Then compare the last element in the sub list (supose it = X) to each subsequent element in main list(supose it = Y), if Y is greater than X :add Y to the last of sub_list and remove Y from the main list, continue until the end of the main_list.
  
	3- After that, merge the existing sub_list to the sorted_list(which is empty at first time), and remove all elements in sub_list.
  
	4- Repeat this until the main list becoming empty

animation:

![Alt Text](/Media/StrandSort.gif)



references :
    Strand Sort:
	https://www.pythonpool.com/python-strand-sort/
	https://en.wikipedia.org/wiki/Strand_sort

   Choose algorithms by this article on geeksforgeeks:
	https://www.geeksforgeeks.org/sorting-algorithms/


