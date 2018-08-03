BINS=setitimer-helper squish-pty squish-unix pintos pintos-gdb pintos-set-cmdline pintos-mkdisk Pintos.pm

all: setitimer-helper squish-pty squish-unix

CC = gcc
CFLAGS = -Wall -W
LOADLIBES = -lm
setitimer-helper: setitimer-helper.o
squish-pty: squish-pty.o
squish-unix: squish-unix.o

install: all
	install $BINS /usr/local/bin

clean: 
	rm -f *.o setitimer-helper squish-pty squish-unix
