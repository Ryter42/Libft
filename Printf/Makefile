# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: emoreau <emoreau@student.42.fr>            +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2023/01/03 21:43:52 by emoreau           #+#    #+#              #
#    Updated: 2023/01/07 04:00:16 by emoreau          ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME = libftprintf.a

SRC =	ft_printf.c\
		printarg.c\
		putnbr.c

FLAG = -Wall\
		-Wextra\
		-Werror

OBJS = $(SRC:.c=.o)

all : $(NAME)

$(NAME) : $(OBJS)
	ar rc $(NAME) $(OBJS)

%.o : %.c
	gcc $(FLAG) -c $<

clean :
	@rm -f *.o

fclean : clean
	@rm -f $(NAME)

re : fclean all

.PHONY : clean fclean re