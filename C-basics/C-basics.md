# **C Basics** 
# What is C?
     Low level programming language
     Used in systems and embedded level programming
     Known for the user being in charge of memory
     Lets you work close to the metal
     Extremely fast 
     One step above assembly
     Compiled language
# Syntax & Structure

```c 
#include <stdio.h>

int main() {
    printf("Hello, world!\n");
   
   return 0;
}
```
# Breakdown

`#include <stdio.h>` invokes functions from the stdio header file which is apart of the C standard library, this allows for printf()

`int main()` the main function, also the start of the program, this will be the first thing the computer executes  
   
`return 0;` returns a value back to the computer letting it know the program was succesful

# Compiling 
`gcc` or `clang` are fine for C

Basic command for compiling a hello.c file
`gcc -o hello hello.c`

`-o` simply means output to this file, with hello.c being the file that needs to be compiled

effectively naming the program **hello**



