# Functions in C
## Definition
A function is a block of code given a name
- Performs a task
- Receives parameters
- Can return a value
Input -> Processing -> Output
```c
int add(int a, int b) {
	return a + b;
}
```


## Anatomy of a Function
```c
return_type function_name(parameters, parameters) {
	// function body
	return value;
}
```

| Part            | Meaning                          |
| --------------- | -------------------------------- |
| `return_type`   | What the function gives back     |
| `function_name` | Identifier used to call function |
| `parameters`    | Inputs                           |
| `{}`            | Scope of the function            |
| `return`        | Sends a value back               |
## Declaring , Defining and Calling
### Declaration
Tells the compiler the functions exists
```c
int foo(int x);
```
### Definition
Contains the actual code
```c
int foo(int x) {
	return x * x; 
}
```
### Calling
Using the Function
```c
int y = foo(5);
```

## Why use Functions?
Avoid repetition
Organize Code
Improve readability

### Bad example
```c
x = a + b;
y = c + d;
z = e + f;
```
### Good example
```c
int add(int x, int y) {
	return x + y;
}

x = add(a, b);
y = add(c, d);
z = add(e, f);
```
