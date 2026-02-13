### Dictionary ADT 
- Search (D, key)
- Insert (D, key, value)
- Delete (D, key)

### AVL Trees 
- A type of BST with an addition of **balance factors** 
	- Balance factors are responsible in keeping the BST balanced, so it solves the worse case of a BST turning into a linked list
- Balance factor is calculated by: $$rightHeight - leftHeight$$
- A tree is considered to be balanced if the different is no greater than 1
- ### Rotations
	- Left rotations
		- Perform when the right subtree is larger than the left subtree 
	- Right rotations 
		- Perform when the left subtree is larger than the right subtree
- #### Double Rotations
	- Perform only when the root BF and the subtree BF are in a **Negative-Positive** relationship
	- The purpose of this is to have the inserted value to be in the outermost subtree, otherwise its going to be unbalanced even after rotation
- 