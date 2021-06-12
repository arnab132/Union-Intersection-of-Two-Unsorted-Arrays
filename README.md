# Union-Intersection-of-Two-Unsorted-Arrays

Given two Unsorted arrays that represent two sets (elements in every array are distinct), find the union and intersection of two arrays.

For example, if the input arrays are: 

arr1[] = {7, 1, 5, 2, 3, 6} 

arr2[] = {3, 8, 6, 20, 7} 

Then your program should print Union as {1, 2, 3, 5, 6, 7, 8, 20} and Intersection as {3, 6, 7}. Note that the elements of union and intersection can be printed in any order.

Union: 

Initialize union U as empty.
Find smaller of m and n and sort the smaller array.
Copy the smaller array to U.
For every element x of larger array, do the following
Binary Search x in the smaller array. If, x is not present, then copy it to U.
Return U.

Intersection: 

Initialize intersection I as empty.
Find smaller of m and n and sort the smaller array.
For every element x of larger array, do the following
Binary Search x in the smaller array. If x is present, then copy it to I.
Return I.

Time complexity of this method is min(mLogm + nLogm, mLogn + nLogn) which can also be written as O((m+n)Logm, (m+n)Logn). 

This approach works much better than the previous approach when the difference between the sizes of two arrays is significant.
