# Arrays in C
## Definition
Arrays are a special kind of variable used to store multiple values in a single variable
This helps with repetitiveness, instead of declaring a bunch of variables we can store them in an array 

The C standard defines them as ***contiguously allocated nonempty set of objects*** meaning, all the elements in the array are stored in a single continuous block of memory, which allows direct access to an element with indexing 
### Characteristics of an Array
- All elements in an array must be of the same data type (all `int` or all `float` etc.)
- Once an array is declared its size cannot be changed
- Elements of the array are accessed with a zero based index , `[0]`is the first element
## Anatomy of an Array
```c
#include <stdio.h>

int main() {

	int arr[] = {1, 3, 5, 7, 9, 13};
	printf("%d", arr[0]); // Accessing the first element and outputting
	return 0;
}
```

| Part        | Meaning                                    |
| ----------- | ------------------------------------------ |
| `int arr[]` | Array of the int data type                 |
| `{1,3,5..}` | The elements of the array (1 is index [0]) |
| `arr[0]`    | Accessing the first element in the array   |
## Changing an Array Element
Simply just refer to the index number of the array and change the value of the element
`myArray[0] = 33`
```c
int my Array[] = {14, 15, 34, 64};
myArray[0] = 33;

printf("%d", myArray[0]); // Outputs 33 instead of 14
```

## Declaring and setting # of Elements
We can actually declare the array before inserting elements, as well as specify the size
```c
int myArray[3];

myArray[0] = 24;
myArray[1] = 78;
myArray[2] = 32;
myArray[3] = 19;
```
[0] is the first index of the element so even though we specified `myArray[3]` C (or the Compiler) counts [0] as the first index so the array is actually 4 elements

## Finding Array Size and # of Elements
To get the size of an array (in bytes, not the sum nor number of elements) simply use the `sizeof`operator
```c
int myArray[] = {12, 32, 42, 64, 100};
printf("%zu", sizeof(myArray));
```
**Output** `20`
`sizeof` returns the size of a type in *bytes* and `int` is usually 4 bytes, 5 elements gives you 20 *bytes*

To get the number of elements in an array  there is a formula or calculation
```c
int myArray[] = {10, 15, 21, 75, 24};
int foo = sizeof(myArray) / sizeof(myArray[0]);
```
**Output** `5`
Basically you are dividing the whole array by the first element of the array giving you the number of elements 