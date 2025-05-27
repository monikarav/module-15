# Exp No : 12
# Binary search tree

## AIM :

To build and evaluate a binary expression tree using recursion in Python, where leaf nodes contain operands and internal nodes contain operators.

## ALGORITHM :

Step 1 : Create Node Structure: Define a Node class with value (val), left, and right children.

Step 2 : Build Expression Tree: Construct the tree with operators as internal nodes and operands as leaves.

Step 3 : Check for Leaf: Define isLeaf() to determine if a node is a leaf (operand).

Step 4 : Evaluate Leaf Nodes: If a node is a leaf, return its float value.

Step 5 : Recursive Evaluation: Recursively evaluate the left and right subtrees.

Step 6 : Apply Operator: Use process() to perform the operator on the evaluated subtrees.

Step 7 : Return Result: Return the final evaluated result from the root node.

## PROGRAM :

```
class Node:
    def __init__(self, val, left=None, right=None):
        self.val = val
        self.left = left
        self.right = right

def isLeaf(node):
    return node.left is None and node.right is None
 
def process(op, x, y):
    if op == '+':
        return x + y
    if op == '-':
        return x - y
    if op == '*':
        return x * y
    if op == '/':
        return x / y
 
def evaluate(root):
    if root is None:
        return 0
    if isLeaf(root):
        return float(root.val)
    
    x=evaluate(root.left)
    y=evaluate(root.right)
    return (process(root.val,x,y))
    
root=Node('+')
root.left=Node('*')
root.right=Node(3)
root.left.left=Node(5)
root.left.right=Node(5)
print("The value of the expression tree is",evaluate(root))

```

## OUTPUT :

![image](https://github.com/user-attachments/assets/0a3eb218-d0f9-4d24-a01a-94e1b496fa5f)

## RESULT :

Thus the building and evaluation of a binary expression tree using recursion in Python, where leaf nodes contain operands and internal nodes contain operators successfully verified.
