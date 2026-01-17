# Operators in C

# Arithmetic Operators

`+`     `Addition`          Adds two values                        `x + y`
`-`     `Subtraction`       Subtracts one value from another       `x -y`
`*`     `Multiplication`    Multiplies two values                  `x * y`
`/`     `Division`          Divides one value by another           `x / y`
`%`     `Modulus`           Returns the division remainder          `x % y`
`++`    `Increment`         Increases the value of a variable by 1 `++x`
`--`    `Decrement`         Decreases the value of a variable by 1 `--x`

If you are looking to get a float number you must use arithmetic with the same data type
- For example: a `int / float` will output an integer while `float / float` will output a float

# Incrementing and Decrementing
Very common in loops, arrays and counters

`++ increases value by 1` `-- decreases by 1`

```c
int x = 5;

++x;  // Increment x by 1
printf("%d\n", x); // 6
```
Output `6`


# Assignment Operators

The most common assignment operator is `=`
```c
int x = 10
```
The addition assignment operator `+=` adds a value to a variable
Same logic can be applied to the rest

`=`     `x = 5`     `x = 5`
`+=`    `x += 3`    `x = x + 3`
`-+`    `x -= 3`    `x = x -3`
