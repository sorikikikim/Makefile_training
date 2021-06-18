NAME = main
SRC = main.c
OBJ = $(SRCS:.c=.o)

LIBFT = libft.a
LIB_NAME = ft
LIB_SRCS = first.c second.c third.c
LIB_OBJS = $(LIB_SRCS:.c=.o)
AR = ar
ARFLAGS = -rc
CC = gcc
CFLAGS = -Wall -Werror -Wextra

.PHONY : all clean fclean 
all : $(NAME)

clean :
	rm -f *.o
fclean : clean
	rm -f $(NAME) $(LIBFT)
re : fclean all

$(NAME) : $(OBJ) $(LIBFT)
	$(CC) $(CFLAGS) -o $@ $^
$(LIBFT) : $(LIB_OBJS)
	$(AR) $(ARFLAGS) $@ $?
%.o : %.c
	$(CC) $(CFLAGS) -c $<

