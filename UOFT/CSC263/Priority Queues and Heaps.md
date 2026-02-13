## Priority Queues
- A list of elements with an extra augmentation of priority. 
- #### Using heap to implement priority queues
	- Represent heap in a list: from top to bottom, left to right in a list
	- The left subtree are located in $$2i$$
	- The right subtree are located in $$2i+1$$
	- From a leaf to parent $$\lfloor \frac{i}{2} \rfloor$$

## Heaps
- Satisfies the heap property
	- The parent nodes are greater than or equal to all of its descendants 
- Satisfies Completeness
	- Each level is full and the last level should be as full as possible from left to right
- #### Complete Binary Tree
	- It's unique, only one possible way to arrange it
- #### Extract max
	- Swap the root and the last leaf
	- Pop the leaf
	- Bubble down by using the larger child
- #### Insert
	- Add it to the end of the heap 
	- Bubble up
	