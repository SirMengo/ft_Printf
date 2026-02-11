*This project has been created as part of the 42 curriculum by msimoes*

## Description
The ft_printf project aims to recreate the function `printf` from the `standard input/output` library of functions. It is an introduction to variadic arguments.

## Instructions
To compile the project, simply run:
```bash
make
```

To recompile everything, run:
```bash
make re
```

This will create a library called `libftprintf.

### Usage
Simply call the function:
```c
ft_printf("String", [optional arguments]);
```

### Arguments
ft_printf will print every argument that will be specified when it is called. To add an argument to what will be printed, it has to be called with `%` followed by a letter that specifies its type. 
Those can be:
- `%c`: char type character
- `%s`: string
- `%p`: pointer to memory address
- `%d` & `%i`: integer
- `%u`: unsigned integer
- `%x`: lower case hexadecimal value
- `%X`: upper case hexadecimal value

To print an `%` it has to be declared as `%%` or else it will be skipped.

### Examples
Basic string printing function:
Example cases:
```c
char *str = "Hello World!";
ft_printf(str);
//Output: Hello World!
```
```c
char *str = "World!";
ft_printf("Hello %s", str);
//Output: Hello World!
```
Basic integer printing function:
```c
int i = 23;
ft_printf("I am %d years old.", i);
//Output: I am 23 years old.
```

### Return value
The ft_printf function will return the number of characters it has written.

### Cleanup
Remove object files:
```bash
make clean
```

Remove object files and the library:
```bash
make fclean
```

## Resources
- [printf manual](https://www.man7.org/linux/man-pages/man3/printf.3.html)
- [Let's build a mini printf function - YouTube Oceano](https://www.youtube.com/watch?v=byRw36Y3Hjs)

### AI usage
No AI was used to write the code of this project.