
## C Language
- Multiplying two integers outputs an integer
- The maximum number that an int can hold is $2^{32}$  
	- Int is 4 Bytes
- Long is 8 bytes 
- Float is 4 bytes
- Double is 8 bytes
- Char is 1 byte

#### Pointers 
- Holds the memory address of the data/variable 
	- Example code: 
	- ```c
	#include <stdio.h>

	int main() {
	    int i;
	    i = 5;
	    printf("Value of i: %d\n", i);
	    printf("Address of i: %p\n", &i);
	    
	    // declare a pointer pt that will point to an int
	    int *pt;
	    // set pt to hold the address of i
	    pt = &i;
	    pt = 9;
	    
	    // print the value of the pointer (which is the address of i)
	    printf("Value of pt: %p\n", pt);
	    // the pointer itself has an address, print that
	    printf("Address of pt: %p\n", &pt);
	
	    // print the value in the address that is itself stored in pt
	    printf("Value pointed to by pt: %d\n", *pt);
	    // should print out 9. Assigning to the pointer variable changes
	    // the variable that it's referring to (i in this case).
	    return 0;
	}
	```
	
	- Use the `&` symbol to assign memory addresses
	- Use `*` when declaring a pointer variable
		- Make sure the datatype of the pointer variable is the same as the variable
		- To dereference a pointer variable, use `*`
- If you **assign a value** to the pointer variable, the pointer **changes the value** of the object that it's **pointing** to 
- Assigning a variable to a new variable keeps the same value in different address
	- Example: 
	- ```c
	  int i = 4; 
	  int j = i; 
	  // Boths stores 4 but in different memory
	  
	  //Interesting example
	  int *pt = q; 
	  // This is equivalent to 
	  int *pt; 
	  pt = q; 
	  ```
- Pointers are used to change out of scope variables within functions. 
	- Example: 
	- ```c
	  /* This function is supposed to lower the grade by one letter-grade. 
 * It doesn't work correctly. 
 */
void apply_late_penalty(char grade) {
   if (grade != 'F') {
       grade++;
   }
}

/* This version works correctly */
void properly_apply_late_penalty(char *grade_pt) {
   if (*grade_pt != 'F') {
       (*grade_pt)++;
   }
}

int main() {
   
    char grade_Michelle = 'B';
    printf("Michelle earned a %c\n", grade_Michelle);

    // We can add 1 to the char 'B' and get the next char in sequence.
    // Since the ASCII codes come in alphabetical order, this would be a 'C'
    grade_Michelle++;   
    printf("Michelle was late, so instead she gets a %c\n",grade_Michelle);

    // Felipe was also late on his assignment but he started with an A
    char grade_Felipe = 'A';
    printf("Felipe earned a %c\n", grade_Felipe);

    //  Let's call a function to lower Felipe's mark.
    apply_late_penalty(grade_Felipe);

    // Felipe's grade didn't change
    printf("Felipe was also late and earns a %c\n",grade_Felipe);


    // Let's call our improved function to lower Felipe's mark
    properly_apply_late_penalty(&grade_Felipe);
    printf("Felipe was also late and earns a %c\n",grade_Felipe);

    return 0;
}
	  ```
- Passing an array into a function only passes the **memory address of the first element** of the array
- #### Pointer Arithmetic
	- Adding a datatype to a pointer will modify the **memory address** of the pointer variable
		- Adding `int` to a pointer will add 4 to the memory address since integer is 8 bytes
		- Adding `char` to a pointer will add 1 to the memory address since char is 1 byte
		- Modifies the memory address according to the size of the datatype being manipulated. 
	- This works with arrays to access different elements of the array since arrays are just a piece of contiguous memory addresses. 
- You can store a pointer in another pointer using multiple `*` 
	- Example code: 
	- ```c
		int main() {

		int i = 81;
		int *pt = &i;
		// Pointer to a pointer *pt
		int **pt_ptr = &pt;
	
		int *r= *pt_ptr;
		int k = *r;
	   
		// We don't actually need the intermediate value r. 
		// We can dereference pt_ptr twice like this.
		int k1 = **pt_ptr;
	  
		// We can even have triple pointers.
		int ***pt_ptr_ptr = &pt_ptr;
		int k2 = ***pt_ptr_ptr;
		return 0;
	}
	  ```

## Linux 
- File: Sequence of bytes stored in some storage media
- File System
- Metadata: The information kept about a file
	- File size, file owner, permissions, last modified time, etc...
- 