# ft_printf - A custom implementation of the printf function

## 📝 Description
The **ft_printf** project is part of the 42 School core curriculum. The goal is to recode the standard C `printf` function. This project teaches the handling of variadic arguments (`va_list`) in C, as well as efficient formatting and output of various data types.

## ✨ Supported Conversions
My implementation of `ft_printf` supports the following format specifiers:

| Specifier | Description |
| :--- | :--- |
| `%c` | A single character. |
| `%s` | A string of characters. |
| `%p` | A pointer address in hexadecimal format. |
| `%d` | A signed decimal integer. |
| `%i` | A signed integer in base 10. |
| `%u` | An unsigned decimal integer. |
| `%x` | A number in hexadecimal (lowercase) format. |
| `%X` | A number in hexadecimal (uppercase) format. |
| `%%` | Prints a percent sign. |

## 🛠️ Installation & Compilation

First, clone the repository:
```bash
git clone https://github.com/Fiona-87327/42Core_ft_printf.git
cd 42Core_ft_printf/ft_printf
```

Compile the library using the provided Makefile:
```bash
make
```
This will generate the static library file `libftprintf.a`.

## 🚀 Usage
To use `ft_printf` in your own project, include the header and link the library during compilation:

```c
#include "ft_printf.h"

int main(void)
{
    ft_printf("Hello %s! The answer is %d.\n", "World", 42);
    ft_printf("Hex check: %x\n", 255);
    return (0);
}
```

Compiling your program:
```bash
cc main.c -L. -lftprintf -o my_program
```

## 📂 Project Structure
- `ft_printf.c`: The main function and the format parser.
- `ft_printf.h`: The header file containing all prototypes.
- `ft_put*.c`: Various helper functions for outputting different data types (Char, String, Hex, Pointer, etc.).
- `Makefile`: Automation of the compilation process.

## 📜 License
This project was developed as part of the 42 curriculum.
