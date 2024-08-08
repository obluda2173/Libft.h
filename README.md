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
memset		| ft_memalloc	| ft_lstnew
bzero		| ft_memdel	| ft_lstdelone
memcpy		| ft_strnew	| ft_lstdel
memccpy		| ft_strdel	| ft_lstadd   
memmove		| ft_strclr	| ft_lstiter
memchr		| ft_striter	| ft_lstmap
memcmp		| ft_striteri	|
strlen		| ft_strmap	|
strdup		| ft_strmapi	|
strcpy		| ft_strequ	|
strncpy		| ft_strnequ	|
strcat		| ft_strsub	|
strlcat		| ft_strjoin	|
strchr		| ft_strtrim	|
strrchr		| ft_strsplit	|
strstr		| ft_itoa	|
strnstr		| ft_putchar	|
strcmp		| ft_putstr	|
strncmp		| ft_putendl	|
atoi		| ft_putnbr	|
isalpha		| ft_putchar_fd	|
isdigit		| ft_putstr_fd	|
isalnum		| ft_putendl_fd	|
isascii		| ft_putnbr_fd	|
isprint		|		|
toupper		|		|
tolower		|		|

Notes:

- All the files and functions are namespaced with an **ft_** in front. It stands for Fourty Two
- The project instructions require that we put all the source files in the root directory.

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

[1]: https://github.com/Matt-Hurd/42-libft/blob/master/libft.en.pdf "Libft PDF"
[2]: http://42.us.org "42 USA"
[3]: https://github.com/R4meau/ "R4meau's Github"
