CFLAGS=-Wall -Werror -Wextra -std=c11
FILE= 1.txt
s21_cat: cat.o
	gcc $(CFLAGS) cat.o -o s21_cat

cat.o:
	gcc $(CFLAGS) -c cat.c

test:
	sh integration_test_cat.sh

all: s21_cat test

clean:
	rm -rf ./*.o
	rm -rf s21_cat

rebuild: clean all
