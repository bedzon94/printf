# 0x11. C - printf

## Description

This team project is part of the Software Engineering (SE) curriculum of ALX School.

What you should learn from this project:

- How to work with a Team
- How to use git in a team setting
- Exploring the uses of _printf
- Managing files and finding a good workflow
- Variadic functions

## Prototype
int _printf(const char *format, ...);

## Compilation
All files were created and compiled on Ubuntu 14.04.4 LTS using GCC 4.8.4 with the command gcc -Wall -Werror -Wextra -pedantic *.c

## Authorized functions and macros
- write (man 2 write)
- malloc (man 3 malloc)
- free (man 3 free)
- va_start (man 3 va_start)
- va_end (man 3 va_end)
- va_copy (man 3 va_copy)
- va_arg (man 3 va_arg)

## TASKS

[0. I'm not going anywhere. You can print that wherever you want to. I'm here and I'm a Spur for life](./_printf.c)
- Write a function that produces output according to a format.
   - Prototype: int _printf(const char *format, ...);
   - Returns: the number of characters printed (excluding the null byte used to end output to strings)
   - write output to stdout, the standard output stream
   - format is a character string. The format string is composed of zero or more directives. See man 3 printf for more detail. You need to handle the following conversion specifiers:
      - c
      - s
      - %
##

[1. Education is when you read the fine print. Experience is what you get if you don't](./print_nums.c)
- Handle the following conversion specifiers:
   - d
   - i

##

[2. Just because it's in print doesn't mean it's the gospel](./man_3_printf)
- Create a man page for your function.

##

[3. With a face like mine, I do better in print](./print_bases.c)
- Handle the following custom conversion specifiers:
   - b: the unsigned int argument is converted to binary
   
```C:
alex@ubuntu:~/c/printf$ cat main.c
#include "main.h"

/**
 * main - Entry point
 *
 * Return: Always 0
 */
int main(void)
{
    _printf("%b\n", 98);
    return (0);
}
alex@ubuntu:~/c/printf$ gcc -Wall -Wextra -Werror -pedantic -std=gnu89 main.c
alex@ubuntu:~/c/printf$ ./a.out
1100010
alex@ubuntu:~/c/printf$

```

##

[4. What one has not experienced, one will never understand in print](./print_bases.c)
- Handle the following conversion specifiers:
   - u
   - o
   - x
   - X

##

[5. Nothing in fine print is ever good news](./write_funcs.c)
- Use a local buffer of 1024 chars in order to call write as little as possible.

##

[7. My weakness is wearing too much leopard print](./print_custom.c)
- Handle the following custom conversion specifier:
   - S : prints the string.
   - Non printable characters (0 < ASCII value < 32 or >= 127) are printed this way: \x, followed by the ASCII code value in hexadecimal (upper case - always 2 characters)

##

[6. How is the world ruled and led to war? Diplomats lie to journalists and believe these lies when they see them in print](./print_address.c)
- Handle the following conversion specifier: p.

##

[8. The big print gives and the small print takes away](./get_flag.c)
- Handle the following flag characters for non-custom conversion specifiers:
   - +
   - space
   - #

##

[9. Sarcasm is lost in print]
- Handle the following length modifiers for non-custom conversion specifiers:
   - l
   - h
   - Conversion specifiers to handle: d, i, u, o, x, X

##

[10. Print some money and give it to us for the rain forests]
- Handle the field width for non-custom conversion specifiers.

##

[11. The negative is the equivalent of the composer's score, and the print the performance]
- Handle the precision for non-custom conversion specifiers.

##

[12. It's depressing when you're still around and your albums are out of print
#advanced]
- Handle the 0 flag character for non-custom conversion specifiers.

##

[13. Every time that I wanted to give up, if I saw an interesting textile, print what ever, suddenly I would see a collection]
- Handle the - flag character for non-custom conversion specifiers.

##

[14. Print is the sharpest and the strongest weapon of our party](./print_custom.c)
- Handle the following custom conversion specifier:
   - r : prints the reversed string

##

[15. The flood of print has turned reading into a process of gulping rather than savoring](./print_custom.c)
- Handle the following custom conversion specifier:
   - R: prints the rot13'ed string

##

[16. *]
- All the above options work well together.





## Contributors

- Norris Selorm Bedzo (bedzon@ieee.org)
- Francis Kwofie (francisskwofie01@gmail.com)


![GitHub contributors](https://img.shields.io/github/contributors/bedzon94/printf)
