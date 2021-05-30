# Union-Intersection-of-Two-Unsorted-Arrays


Intersection: 

Initialize intersection I as empty.
Find smaller of m and n and sort the smaller array.
For every element x of larger array, do the following
Binary Search x in the smaller array. If x is present, then copy it to I.
Return I.

Time complexity of this method is min(mLogm + nLogm, mLogn + nLogn) which can also be written as O((m+n)Logm, (m+n)Logn). This approach works much better than the previous approach when the difference between the sizes of two arrays is significant.
