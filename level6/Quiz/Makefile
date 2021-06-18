NAME = libft.a
SRCS = first.c \
	   second.c \
	   third.c
OBJS = $(SRCS:.c=.o)
AR = ar
ARFLAGS = -rc
CC = gcc
CFLAGS = -Wall -Werror -Wextra

all : $(NAME)

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $?

%.o : %.c
	$(CC) $(CFLAGS) -c $<

clean :
	rm -f *.o
fclean : clean
	rm -f $(NAME)
re : fclean all

.PHONY : all clean fclean 
