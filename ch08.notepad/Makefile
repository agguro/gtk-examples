all: notepad

# Compiler settings
CC = gcc -Wall -O `gtk-config --cflags`

main.o: main.c 
	$(CC) -c -g main.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

notepad.o: notepad.c 
	$(CC) -c -g notepad.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

filesel.o: filesel.c 
	$(CC) -c -g filesel.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

about.o: about.c 
	$(CC) -c -g about.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

menu.o: menu.c 
	$(CC) -c -g menu.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

progressbar.o: progressbar.c 
	$(CC) -c -g progressbar.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

search.o: search.c 
	$(CC) -c -g search.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

rtfreadr.o: rtfreadr.c 
	$(CC) -c -g rtfreadr.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

rtfactn.o: rtfactn.c 
	$(CC) -c -g rtfactn.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`
	
misc.o: misc.c 
	$(CC) -c -g misc.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

showmessage.o: showmessage.c 
	$(CC) -c -g showmessage.c `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`
	
	
# Object modules
OBJS = main.o notepad.o filesel.o about.o menu.o misc.o progressbar.o search.o rtfreadr.o rtfactn.o showmessage.o

notepad:  main.o notepad.o filesel.o about.o menu.o misc.o progressbar.o search.o rtfreadr.o rtfactn.o showmessage.o
	gcc -o notepad $(OBJS) `pkg-config --cflags gtk+-2.0 --libs gtk+-2.0`

.PHONY:
clean:
	@rm -f $(OBJS) notepad
