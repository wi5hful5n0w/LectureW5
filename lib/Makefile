.PHONY:clean info
CC = gcc
CFLAGS = -g -Wall
OBJFILES = func1.o func2.o
INCLUDE = ../include
OUTPUT = libfuncs.a

$(OUTPUT): $(OBJFILES)
	ar rv $(OUTPUT) $(OBJFILES)
%.o: %.c
	$(CC) $(CFLAGS) -I$(INCLUDE)  -c $< -o $@
clean:
	sudo rm *.o $(OUTPUT)
info:
	nm libfuncs.a
