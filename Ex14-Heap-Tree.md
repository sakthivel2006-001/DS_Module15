# Ex14 Heap Tree
## DATE:19-03-2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
```
1.Start
2.Find the index of the element num in the array.
3.Swap the element to be deleted with the last element in the array.
4.Decrease the array size (size) by 1.
5.Start heapifying from the last non-leaf node (index size/2 - 1).
6.Call heapify() to restore the heap property for each node.
7.End
```
## Program:

### Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

#### DEVELOPED BY:SAKTHIVEL S
#### REGISTER NO:212223220090
```
struct n { 
char d; 
struct n *l; 
struct n *r; 
};
void preOrder(struct n *tree) 
{ 
if(tree) 
{ 
printf("%c",tree->d); 
preOrder(tree->l); 
preOrder(tree->r); 
} 
} 
void inOrder(struct n *tree) 
{ 
if(tree) 
{ 
inOrder(tree->l); 
printf("%c",tree->d); 
inOrder(tree->r); 
} 
} 
void postOrder(struct n *tree) 
  
  
{ 
if(tree) 
{ 
postOrder(tree->l); 
postOrder(tree->r); 
printf("%c",tree->d); 
} 
} 
```

## Output:
![image](https://github.com/user-attachments/assets/5d2990ad-11ab-42d0-aa67-48f358ea3597)



## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
