CC = g++
CFLAGS = -Wall -c


all: app

app: main.o liboper.a
	$(CC) main.o liboper.a -o app

liboper.a: add.o mul.o
	ar rcs liboper.a add.o mul.o

%.o: %.cpp oper.hpp
	$(CC) $(CFLAGS) $<

clean:
	rm -rf *.o app liboper.a
