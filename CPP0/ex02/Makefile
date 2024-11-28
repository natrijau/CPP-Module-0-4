NAME=megaphone
CXX=c++
CXXFLAGS=-std=c++98 -Wall -Wextra -Werror -g
SRCS=megaphone.cpp
OBJS=$(SRCS:.cpp=.o)

all: $(NAME)

$(NAME): $(OBJS)
	@$(CXX) $(OBJS) -o $(NAME)
	@echo "\n\nmegaphone builded"

%.o: %.cpp
	@$(CXX) $(CXXFLAGS) -c $< -o $@
	@echo -n '.....'

clean:
	@rm -f $(OBJS)
	@echo "All objects clean"

fclean: clean
	@rm -f $(NAME)
	@echo "And the executable too"

re: fclean all

.PHONY: all fclean clean re