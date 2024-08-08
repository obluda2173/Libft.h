# Libft.h - erian
Welcome to libft, a custom C library that serves as a foundation for various 42 projects.
## TOC
- [What is libft?](#what-is-libft)
- [What's in it?](#whats-in-it)
- [How does it work?](#how-does-it-work)
- [How do I use the library?](#how-do-i-use-the-library)
- [Example usage](#example-usage)

### What is libft?
[Libft][1] is an individual project at [42][2] that requires us to re-create some standard C library functions including some additional ones that can be used later to build a library of useful functions for the rest of the program.

We re-create these functions in order to deepen our understanding of C. The general philosophy of 42 is that it's best to fully understand that machine that you're using and how it all works together. As a result, we avoid treating even these basic functions as black-boxes.

### What's it do?

As you can see from the [Project instructions][1], there are 3 sections:

1.  **Libc Functions:** Some of the standard C functions
2.  **Additional functions:** Functions 42 deems will be useful for later projects
3.  **Bonus Functions:** Functions 42 deems will be useful for linked lists

Libc functions | Additional functions | Bonus Functions
:----------- | :-----------: | :-----------: 
ft_isalpha.c	| ft_substr.c	| ft_lstlast.c
ft_isdigit.c	| ft_strjoin.c	| ft_lstnew.c
ft_isalnum.c	| ft_strtrim.c	| ft_lstmap.c
ft_isascii.c	| ft_split.c	| ft_lstsize.c
ft_isprint.c	| ft_itoa.c	| ft_lstadd_back.c
ft_strlen.c	| ft_strmapi.c	| ft_lstadd_front.c
ft_memset.c	| ft_striteri.c	| ft_lstiter.c
ft_bzero.c	| ft_putchar_fd.c	| ft_lstdelone.c
ft_memmove.c	| ft_putstr_fd.c	| ft_lstclear.c
ft_strlcpy.c	| ft_putendl_fd.c	|
ft_strlcat.c	| ft_putnbr_fd.c	|
ft_toupper.c	| 	|
ft_tolower.c	| 	|
ft_strchr.c	| 	|
ft_strrchr.c	| 	|
ft_strncmp.c	| 	|
ft_memchr.c	| 	|
ft_memcmp.c	| 	|
ft_strnstr.c	| 	|
ft_atoi.c	| 	|
ft_calloc.c	| 	|
ft_strdup.c	| 	|

### How does it work?

The goal is to create a library called libft.a from the source files so I can later use that library from other projects at 42.

To create that library, after downloading/cloning this project, **cd** into the project and call make:

	git clone https://github.com/obluda2173/Libft.h.git
	cd libft.h
	make

You should see a *libft.a* file and some object files (.o).


Now to clean up (removing the .o files), call `make clean`

### How do I use the library?

When compiling, you have to tell the file where your library resides and which library it is using:

`gcc -L. -lft -o example.out example.c`

-L takes the path to your library. `.` in this case<br>
-l takes the name of your library. This is the set of characters that come after `lib` in your library name.

That's it. Now run it using `./example.out`

Hope this was useful.

###Inspiration:
- [Description][3]
- [Tests][4]
- [Comparison (with bonuses)][5]
- [Readme greates inspiration][6]


[1]: https://github.com/obluda2173/Libft.h/blob/main/libft.pdf "libft.pdf"
[2]: https://42.fr/en/homepage/
[3]: https://medium.com/@piolodale/libft-42-cursus-871329cc51d3#:~:text=ft_memset()%20and%20ft_bzero(),pointers%20in%20the%2042%20cursus.
[4]: https://github.com/xicodomingues/francinette
[5]: https://github.com/markveligod/libft/blob/master/Makefile
[6]: https://github.com/Matt-Hurd
