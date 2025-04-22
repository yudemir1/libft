# Libft 📚 (42 School Project)

My first custom C library, a fundamental project in the 42 curriculum. This library contains reimplementations of standard C functions (libc) and additional useful utilities, designed to be a reusable toolkit for future C projects.

---

## 🎯 Goal

To gain a deeper understanding of standard C functions by implementing them from scratch and to create a personal, reliable library of common utilities for use in subsequent 42 school assignments.

---

## ✨ Features

The library is organized into mandatory and bonus parts:

### Part 1: Reimplemented Libc Functions

Careful reimplementations of functions found in the standard C library, behaving identically to the originals (as per `man` pages). Examples include:

*   **Character:** `ft_isalpha`, `ft_isdigit`, `ft_isalnum`, `ft_isascii`, `ft_isprint`, `ft_toupper`, `ft_tolower`
*   **String:** `ft_strlen`, `ft_strlcpy`, `ft_strlcat`, `ft_strchr`, `ft_strrchr`, `ft_strncmp`, `ft_strnstr`, `ft_strdup`
*   **Memory:** `ft_memset`, `ft_bzero`, `ft_memcpy`, `ft_memmove`, `ft_memchr`, `ft_memcmp`, `ft_calloc`
*   **Conversion:** `ft_atoi`

*(See `libft.h` for the complete list)*

### Part 2: Additional Utility Functions

Helpful functions not found in the standard libc or implemented with different behavior. Examples include:

*   `ft_substr`: Extracts a substring.
*   `ft_strjoin`: Concatenates two strings.
*   `ft_split`: Splits a string by a delimiter into an array.
*   `ft_itoa`: Converts an integer to a string.
*   `ft_strmapi`: Creates a new string by applying a function to each character.
*   `ft_striteri`: Applies a function to each character of a string.
*   `ft_putchar_fd`, `ft_putstr_fd`, `ft_putendl_fd`, `ft_putnbr_fd`: Write data to a specific file descriptor.

*(See `libft.h` for the complete list)*

### Bonus: Linked List Functions

Functions to create and manipulate a generic singly linked list (`t_list`).
*(Mark `[x]` if implemented)*

*   `[ ]` Implemented:
    *   `ft_lstnew`: Creates a new list element.
    *   `ft_lstadd_front`: Adds an element to the beginning.
    *   `ft_lstadd_back`: Adds an element to the end.
    *   `ft_lstsize`: Counts the number of elements.
    *   `ft_lstlast`: Returns the last element.
    *   `ft_lstdelone`: Deletes a single element.
    *   `ft_lstclear`: Deletes all elements and frees memory.
    *   `ft_lstiter`: Applies a function to each element's content.
    *   `ft_lstmap`: Creates a new list by applying a function to each element.

---

## 💻 Tech Stack

*   **Language:** `C`
*   **Compiler:** `cc` (with `-Wall -Wextra -Werror` flags)
*   **Build System:** `Make`
*   **Archiver:** `ar` (to create the static library `libft.a`)

---

## 🚀 Usage

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/yudemir1/libft.git
    cd libft
    ```

2.  **Compile the library:**
    *   To compile only the mandatory functions:
        ```bash
        make
        ```
    *   To compile both mandatory and bonus functions (if available):
        ```bash
        make bonus
        ```
    This will create the `libft.a` static library file.

3.  **Use in your project:**
    *   Copy the `libft.a` file and the `libft.h` header file into your own project directory.
    *   Include the header in your C files: `#include "libft.h"`
    *   When compiling your project, link against the library:
        ```bash
        cc your_project.c -L. -lft -o your_executable
        # Or if libft.a is in a subdirectory 'libft':
        # cc your_project.c -L./libft -lft -o your_executable
        ```

---
