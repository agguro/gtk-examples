
CC = gcc

PROGS = sortlist tree hash message list mem

all: $(PROGS)

sortlist: sortlist.c 
	$(CC) -o sortlist sortlist.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0` 

tree: tree.c 
	$(CC) -o tree tree.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

hash: hash.c
	$(CC) -o hash hash.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

message: message.c
	$(CC) -o message message.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

list: list.c
	$(CC) -o list list.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

mem: mem.c
	$(CC) -o mem mem.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

IGNORED = *.o $(PROGS)

.PHONY:
ignored:
	@echo $(IGNORED)

.PHONY:
clean:
	rm -f *.o $(PROGS)
