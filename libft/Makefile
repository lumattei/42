RM = rm -rf

LIBC = 	ft_isalpha.c	ft_isdigit.c	ft_isalnum.c	ft_isascii.c\
		ft_isprint.c	ft_strlen.c		ft_memset.c		ft_bzero.c\
		ft_memcpy.c		ft_memmove.c	ft_strlcpy.c	ft_strlen.c\
		ft_strlcat.c

SRCS = ${LIBC}

OBJ = $(SRCS:.c=.o)

NAME = libft.a

CC = gcc

CFLAGS = -Wall -Werror -Wextra

%.o : %.c
	$(CC) $(CFLAGS) -o $@ -c $<

${NAME}: ${OBJ}
	ar -rsc ${NAME} ${OBJ}

all : $(NAME)

clean :
	$(RM) $(OBJ)

fclean : clean
	$(RM) $(NAME)

re : fclean all

.PHONY: all re clean fclean
