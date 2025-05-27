# Exp No : 13 
# Binary tree

## AIM :

To build and display a binary tree using integer or string values input by the user with the help of the binarytree module's Node class.

## ALGORITHM :

Step 1 : Import Library: Import Node class from the binarytree module.

Step 2 : Initialize List: Create an empty list l to store node values.

Step 3 : Get User Input: Read 3 values (root, left, and right) from the user and append them to the list.

Step 4 : Create Tree: Create the root node using the first value, and assign its left and right children using the second and third values.

Step 5 : Print Tree: Traverse the tree using the built-in .values property of the Node object to print all values in the tree.

Step 6 : Display Format: Print values in a formatted "value -->" style.

## PROGRAM :

```
from  binarytree      import Node
l=[]
for i in range(0,3):
    a=input()
    l.append(a)
root=Node(l[0])
root.left=Node(l[1])
root.right=Node(l[2])
print("Binary Tree : ")
for i in root.values:
    print(i,"--> ",end="")
```

## OUTPUT : 

![image](https://github.com/user-attachments/assets/c66967dd-320f-4902-85fa-844abfbb0f9c)

## RESULT : 

Thus the building and displaying a binary tree using integer or string values input by the user with the help of the binarytree module's Node class si successfully verified.

