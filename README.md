﻿# Merge-Sort

#### Step 1: 
Prompt the user to input the size of the array (\( n \))  
- Input the value of \( n \).  

#### Step 2:
Declare an array of size \( n \)  
- Create an array \( arr \) of size \( n \).  

#### Step 3: 
Input array elements  
- Loop from \( i = 0 \) to \( n-1 \).
- Input \( arr[i] \) for each iteration.  

#### Step 4: 
Call the `mergeSort` function to sort the array  
- Pass the array, along with its start index (\( l = 0 \)) and end index (\( r = n-1 \)), to the `mergeSort` function.  

#### Step 5: 
In the `mergeSort` function, if \( l < r \)  
- Calculate the middle index:
   \[
   m = l + \frac{(r - l)}{2}
   \]
- Recursively call `mergeSort` on the left half:
   - \( mergeSort(arr, l, m) \).
- Recursively call `mergeSort` on the right half:
   - \( mergeSort(arr, m+1, r) \).
- Call the `merge` function to merge the two halves:
   - \( merge(arr, l, m, r) \).


#### Step 6: 
In the `merge` function  
1. Create two temporary arrays:
   - \( L \) for elements \( arr[l \, ... \, m] \).
   - \( R \) for elements \( arr[m+1 \, ... \, r] \).
2. Copy the elements from \( arr \) into \( L \) and \( R \).  

#### Step 7: 
Merge the temporary arrays \( L \) and \( R \) 
1. Use three pointers:
   - \( i \) for traversing \( L \).
   - \( j \) for traversing \( R \).
   - \( k \) for updating \( arr \).
2. Compare elements from \( L \) and \( R \):  
   - If \( L[i] \leq R[j] \), set \( arr[k] = L[i] \) and increment \( i \).  
   - Otherwise, set \( arr[k] = R[j] \) and increment \( j \).  
3. Increment \( k \) after placing an element in \( arr \).  

#### Step 8: 
Copy any remaining elements 
- If there are leftover elements in \( L \), copy them into \( arr \).  
- If there are leftover elements in \( R \), copy them into \( arr \).  

#### Step 9: 
Print the sorted array
- Loop from \( i = 0 \) to \( n-1 \).  
- Print \( arr[i] \) for each iteration.  

#### Step 10: 
Terminate the program 

