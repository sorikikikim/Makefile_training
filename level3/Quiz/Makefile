NAME = libft.a
SRCS = first.c \
	   second.c \
	   third.c
OBJS = first.o \
	   second.o \
	   third.o
AR = ar
ARFLAGS = -rc

$(NAME) : $(OBJS)
	$(AR) $(ARFLAGS) $@ $?
	//$? vs $^
	//$? 타임스탬프 검사해서 반영(새로운 전제 조건)
	//$^ 모든 전제조건 