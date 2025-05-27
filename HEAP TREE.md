# Exp No : 11
# Tree representation and traversal 

## AIM :

To implement the pushpop operation on a heap tree using Python's heapq module.

## ALGORITHM :

Step 1 : Initialize a Heap: Start with an existing list of elements that represent a min-heap.

Step 2 : Heapify the List: Use heapq.heapify() to convert the list into a valid min-heap.

Step 3 : Input from User: Get the new value to be pushed into the heap from the user.

Step 4 : Push and Pop Operation: Use heapq.heapreplace() to push the new element and pop the smallest element from the heap in a single operation.

Step 5 : Display Results: Print the heap after the pushpop operation.

## PROGRAM : 

```
import heapq
li=[4, 6, 15, 10, 8, 18, 21]
heapq.heapify(li)
print("The created heap is : ",li)
a=int(input())
heapq.heapreplace(li,a)
print("Heap after pushpop operation: ",li)
```

## OUTPUT : 

![image](https://github.com/user-attachments/assets/7d0c536f-a085-4df2-bdee-676e593f312b)

## RESULT :

Thus the implementation of pushpop operation on a heap tree using Python's heapq module.
