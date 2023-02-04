
![[Tree Data Structure.png]]
Node height = max distance from node to the leaf node in that nodes children

Types of tree:
- Binary Tree

Binary Tree

```ad-note
title: Binary Tree

Maximum number of children a node can have is 2
```

Binary Search Tree

```ad-note
title: Binary Search Tree

Binary tree with the nodes thaty are sorted
```
left node < parent node 
![[Binary Search Tree rule 1.png|275]]
right node > parent node 
![[Binary Search Tree rule 2.png|275]]
all left nodes < parent node 
![[Binary Search Tree rule 3.png|275]]
all right nodes > parent node 
![[Binary Search Tree rule 4.png|275]]

Searching element 
go to left child node if search value is less than the current node, repeat until value is found
if search value is higher then current node go to right child node, repeat until value is found 



Unbalanced Trees
- More like a linked list 

Balanced Trees 
- has both right and left child node 
![[Binary Search Tree Type.png]]

![[Binary Search Tree orders.png]]