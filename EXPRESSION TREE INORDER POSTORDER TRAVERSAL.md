# Exp No : 15 
# SEB 

## Aim

To Write a python program to implement push and pop an element into the below given Heap tree using a single built-in function.

## Algorithm

1. Start the program.
   
2. Import heapq Module: Import the heapq module to use heap operations.

3. Initialize List: Define a list li with given integer elements.

4. Convert to Heap: Use heapq.heapify(li) to convert the list into a min-heap in-place.

5. Display Heap: Print the heapified list.

6. Take Input: Read an integer a from the user.

7. Heap Replace: Use heapq.heapreplace(li, a) to replace the smallest element with a (pop and push in one step).

8. Display Updated Heap: Print the modified heap after the heapreplace operation.

9. Stop the program.

## Program

```
import heapq
li=[4, 6, 15, 10, 8, 18, 21]
heapq.heapify(li)
print("The created heap is : ",li)
a=int(input())
heapq.heapreplace(li,a)
print("Heap after pushpop operation: ",li)
```

## OUTPUT

![image](https://github.com/user-attachments/assets/8936aafa-c53b-487f-af67-c896cb29ddd9)

## RESULT

Thus the python program to implement push and pop an element into the below given Heap tree using a single built-in function was successfully implemented.
