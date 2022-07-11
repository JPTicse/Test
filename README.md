# Printf

## Synopsis
This is a simple implementation of printf function that formats and prints data

## Description
The _printf() function produces output according to a format which is described
below. This function write its output to the stdout, the standard output stream. Returns the count of printed characters when the function is successful and -1 when the function fails.

The available convertion specifiers are:
+ %c: Prints a single character.
+ %s: Prints a string of characters.
+ %%: Prints percent.
+ %d: Prints integers.
+ %i: Prints integers.

## Usage
+ All the files are to be compiled on Ubuntu 20.04 LTS
+ Compile your code with "gcc -Wall -Werror -Wextra -pedantic -std=gnu89 -Wno-format *.c"
+ Include the "main.h" header file on the functions using the _printf()

## Example

```
#include "main.h"
#include <limits.h>
#include <stdio.h>

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    int len;
    int len2;

    len = _printf("Let's try to printf a simple sentence.\n");
    len2 = printf("Let's try to printf a simple sentence.\n");
    _printf("Length:[%d, %i]\n", len, len);
    printf("Length:[%d, %i]\n", len2, len2);
    _printf("Negative:[%d]\n", -762534);
    printf("Negative:[%d]\n", -762534);
    _printf("Character:[%c]\n", 'H');
    printf("Character:[%c]\n", 'H');
    _printf("String:[%s]\n", "I am a string !");
    printf("String:[%s]\n", "I am a string !");
    len = _printf("Percent:[%%]\n");
    len2 = printf("Percent:[%%]\n");
    _printf("Len:[%d]\n", len);
    printf("Len:[%d]\n", len2);
    return (0);
}
```

## Autors
| [<img src="https://avatars.githubusercontent.com/u/100174476?v=4" width=115><br><sub> Wilson Valer </sub>](https://github.com/WilsonValer) |  [<img       src="https://avatars.githubusercontent.com/u/101225802?v=4" width=115><br><sub>Aaron Jauregui </sub>](https://github.com/aaronJau21) |
| :---: | :---: | 
