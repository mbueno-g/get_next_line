# get_next_line

WIP 🚧

:books: [Introduction](#introduction)

:collision: [New concept](#new-concept): File descriptor + buffer size + static variables

:footprints: [Step by step](#step-by-step)

<!-- :bookmark_tabs: [Push_swap example](#push_swap-example)

:collision: [New concept](#new-concept): Bitwise operators

:footprints: [My sorting algorithm](#my-sorting-algorithm) -->

## Introduction 

The aim of the get_next_line proyect is to write a function that returns a line read from a file descriptor. What we call a line is a succession of characters that end with '\n' (newline) or with EOF (End Of File).
The prototype of the function to code is:
```C
char  *get_next_line(int fd);
```
The only parameter is a file descriptor of the file we want to read line by line and the return value is the read line or NULL if any error occurs.


## New concept
### File descriptor
A file descriptor (fd) is a non-negative integer number that uniquely identifies an open file in a Unix-like computer operating systems. 
There're three standards file descriptors:

| Integer value | Name | <unistd.h> |
| :------------:| :---:| :--------: |
0 | Standard input | STDIN_FILENO
1 | Standard output | STDOUT_FILENO
2 | Standard error | STDERR_FILENO

There's a limit of file descriptors depending on the operating system. Under Linux, this limit is 4096, meaning we can't open more than 4096 
files at the same time. 

### Buffer size
The buffer size is the amount of characters that our program is reading at one.
Our program must compile with the flag -D BUFFER_SIZE=XX to change the value of the buffer size macro.
sta

### Static variables
Static variables are a unique type of variables with some special properties 
They are able to preserve their value even after they are out of their scope (i.e. the static variable remains in memory while the program is running), so they are not initialized again in a new scope.

The syntax is:
```C
static <data type> <var name>;
```

## Step by step


