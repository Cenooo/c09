SRCS	= srcs/ft_putchar.c srcs/ft_swap.c srcs/ft_putstr.c srcs/ft_strlen.c srcs/ft_strcmp.c 

OBJS	= ${SRCS:.c=.o}

NAME	= libft.a

${NAME}:	${OBJS}
			ar rc ${NAME} ${OBJS} ${LDFLAGS}	

CC	= gcc

RM	= rm -f

CFLAGS	= -Wall -Wextra -Werror 

LDFLAGS	= includes/ft.h

all:	libft.a

libft.a :	${NAME}

.c.o:
	${CC} ${CFLAGS} -c $< -o ${<:.c=.o}

clean:
	${RM} ${OBJS}

fclean:	clean
	${RM} ${NAME}
	
re:	fclean all
