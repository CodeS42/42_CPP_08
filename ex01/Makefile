SRCS =  srcs/main.cpp \
		srcs/Span.cpp 

OBJS = $(SRCS:.cpp=.o)

INCLUDES = headers

NAME = Span

FLAGS = -Wall -Wextra -Werror -std=c++98

.cpp.o :
		c++ $(FLAGS) -I $(INCLUDES) -c $< -o $@

all : $(NAME)

$(NAME) : $(OBJS)
		c++ $(OBJS) -o $(NAME)

clean :
		rm -f $(OBJS)

fclean : clean
		rm -f $(NAME)

re : fclean all

.PHONY : all clean fclean re