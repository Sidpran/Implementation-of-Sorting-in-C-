# Implementation-of-Sorting-in-C-

Aim: To explore and implement various sorting algorithms in C++

Software: -Mingw C/C++ compiler
          -VS Code
          -online C++ compiler

# Program 1. Bubble sort using pointer
Theory with explanation of the code:

- Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order.  
- This implementation uses pointers to traverse the array, incrementing pointer addresses instead of array indices.  
- The outer loop determines the number of passes, while the inner loop compares `*ptr` and `*(ptr+1)`.  
- Swapping is performed through dereferencing pointers (`*a`, `*b`).  
- Pointer arithmetic allows for low-level memory control.  
- Sorting is **in-place**, using O(1) extra space.  
- Time complexity is O(n²) for both average and worst-case scenarios.  
- This approach is suitable for environments with limited memory or embedded systems.

Algorithm:  
- Start  
- Repeat the process for `(n - 1)` passes, where `n` is the array size.  
- In each pass, set a pointer to the current element and another to the next element.  
- Compare the two values.  
- If the first value is greater than the second, swap them using a temporary variable.  
- Move both pointers one step forward.  
- Continue until the end of the unsorted portion.  
- After each pass, reduce the comparison range by one.  
- Repeat steps 3–7 until all elements are sorted.  
- End

# Program 2. Insertion sort
Theory with explanation of the code:

- Insertion Sort builds the sorted array one element at a time.  
- It assumes the first element is already sorted.  
- Each new element (key) is compared with the sorted portion to find its correct position.  
- Elements larger than the key are shifted one position to the right.  
- Sorting is **in-place**, with O(1) extra space.  
- Time complexity: O(n²) for average/worst cases, O(n) for best case (already sorted).  
- The algorithm is stable and preserves the order of equal elements.  
- Efficient for small or nearly sorted datasets and simple to implement.

Algorithm:  
- Start  
- Select the current element as the key.  
- Compare it with the sorted portion to its left.  
- Shift all larger elements one position right.  
- Insert the key at its correct position.  
- Repeat steps 2–5 for all elements in the array.  
- End

# Program 3. Bubble sort
Theory with explanation of the code:

- Bubble Sort compares adjacent elements and swaps them if they are out of order.  
- Multiple passes continue until the array is completely sorted.  
- Elements are accessed either using pointers or array indices.  
- The outer loop counts the passes; the inner loop performs the comparisons.  
- After each pass, the largest unsorted element moves to its correct position.  
- Sorting is **in-place**, with O(1) extra space.  
- Time complexity: O(n²) in average and worst cases.  
- The algorithm is simple, stable, and ideal for understanding pointer manipulation and basic sorting logic.

Algorithm:  
- Start  
- Input the number of elements and store them in an array.  
- Initialize a pass counter.  
- Repeat the sorting process for all passes.  
- In each pass, compare adjacent elements using pointers or indices.  
- If the first element is larger, swap it with the second.  
- Continue until the end of the unsorted portion.  
- Increment the pass counter.  
- Repeat until the array is sorted.  
- Display the sorted array.  
- End

# Conclusion
These three sorting implementations—**Pointer-based Bubble Sort, Array-based Bubble Sort, and Insertion Sort**—highlight fundamental algorithmic techniques.  

- Pointer-based Bubble Sort emphasizes memory manipulation and low-level control.  
- Array-based Bubble Sort offers clarity and simplicity for beginners.  
- Insertion Sort efficiently places elements and is suitable for nearly sorted datasets.  

All three algorithms are **in-place** and **stable**, making them memory-efficient and predictable.  
While not optimal for very large datasets, these implementations are excellent for learning sorting logic, control flow, and data movement, building a strong foundation for more advanced algorithms.
