CC = gcc
INCLUDE = .
CFLAGS = -g -Wall
makefile: main.o dog.o turtle.o blackcow.o
	$(CC) -o animal.exe  main.o dog.o turtle.o blackcow.o
dog.o: dog.c animal.h
	$(CC) -I$(INCLUDE) $(CFLAGS) -c  dog.c
main.o: main.c animal.h
	$(CC) -I$(INCLUDE) $(CFLAGS) -c  main.c
turtle.o: turtle.c animal.h
	$(CC) -I$(INCLUDE) $(CFLAGS) -c turtle.c
blackcow.o: blackcow.c animal.h
	$(CC) -I$(INCLUDE) $(CFLAGS) -c blackcow.c
.PHONY: clean
clean:
	rm -f *.o $(TARGET)
