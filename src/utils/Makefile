
all: setitimer-helper squish-pty squish-unix

INSTALL_FILES=setitimer-helper squish-pty squish-unix pintos pintos-gdb pintos-set-cmdline pintos-mkdisk Pintos.pm

CC = gcc
CFLAGS = -Wall -W
LOADLIBES = -lm
setitimer-helper: setitimer-helper.o
squish-pty: squish-pty.o
squish-unix: squish-unix.o

install: all
	install $(INSTALL_FILES) /usr/local/bin

clean: 
	rm -f *.o setitimer-helper squish-pty squish-unix
