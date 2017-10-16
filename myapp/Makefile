.PHONY: clean info
CC = gcc
CFLAGS = -g -Wall
INCLUDE = ../include
LIBRARY = ../lib
OUTPUT = main

main:main.o
	$(CC) $(CFLAGS) -o $(OUTPUT) -L$(LIBRARY) main.o -lfuncs
main.o:main.c
	$(CC) $(CFLAGS) -c -I$(INCLUDE) main.c -o main.o
clean:
	sudo rm *.o $(OUTPUT)
info:
	nm main
	
