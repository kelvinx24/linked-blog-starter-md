## Full Binary Trees
Binary trees with nodes with two child nodes or no child nodes
 ![[pict_14.png]]

### Heap
Heap rules
- Max value at root 
- Every value in the both the left and right subtrees of a node must be less than or equal to the value at the node
- Both the left and right subtrees must themselves be valid heaps.
- The subnodes of a heap cannot be compared
- Every level except the deepest must contain as many nodes as possible; at the deepest level all the nodes are as far left as possible.

To fix a heap after removal of root
- Right-most node at bottom-most level is removed b/c of last heap rule
	- Can be found at Array size - 1
- O(logn)

#### Heap Sort
- O(nlogn)
- Keep getting right-most node


![[pict_15.png]]