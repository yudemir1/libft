libft (42 School Project)

My first C library, containing reimplementations of standard C functions (libc) and additional useful utilities.

Goal: To create a personal library of common C functions to be reused in future 42 projects.

Includes:

    Part 1 (Libc Functions): Reimplementations of functions like ft_isalpha, ft_isdigit, ft_strlen, ft_memcpy, ft_memset, ft_strlcpy, ft_atoi, ft_calloc, ft_strdup, etc.

    Part 2 (Additional Functions): Useful functions not in libc or with different behavior, such as ft_substr, ft_strjoin, ft_split, ft_itoa, ft_putnbr_fd, etc.

    Bonus (Linked List Functions): Functions to manipulate a generic linked list (ft_lstnew, ft_lstadd_front, ft_lstadd_back, ft_lstsize, ft_lstclear, etc.). (Mark [x] if implemented)

Tech: C, Make, ar (for library creation)

Usage:
    git clone https://github.com/yudemir1/libft.git
    cd libft
    make && make bonus (if you are going to use bonus parts)
