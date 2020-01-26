
Resizeable-Array:In computer science, a dynamic array, growable array, resizable array, dynamic table, mutable array, or array list is a random access, variable-size list data structure that allows elements to be added or removed. It is supplied with standard libraries in many modern mainstream programming languages.

#IMPLEMENTATION

The key is to provide means to grows an array A that stores the elements of a list. We can’t actually grow the array, its capacity is fixed. If an element is appended to a list at a time, when the underlying array is full, we need to perform following steps.

1.Allocate a new array B with larger capacity (A commonly used rule for the new array is to have twice the capacity of the existing array)
2.Set B[i]=A[i], for i=0 to n-1 where n denotes the current no of items.
3.Set A=B that is, we hence forth use B as the array of supporting list.
4.Insert new element in the new array.

#Function Implementation

(1).Len:Return number of elements sorted in array 
(2).get_item: Return element at index k and Check it k index is in bounds of array and Retrieve from the array at index k 
(3).append:Add element to end of the array and assign New bigger array and reset the capacity according to it need.
(4).make_array:Returns a new array with new_cap capacity
