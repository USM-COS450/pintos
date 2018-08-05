
all: setitimer-helper squish-pty squish-unix

INSTALL_FILES=setitimer-helper squish-pty squish-unix pintos pintos-gdb pintos-set-cmdline pintos-mkdisk Pintos.pm

INSTALL_DIR ?= DSTDIR

CC = gcc
CFLAGS = -Wall -W
LOADLIBES = -lm
setitimer-helper: setitimer-helper.o
squish-pty: squish-pty.o
squish-unix: squish-unix.o

install: all
	install $(INSTALL_FILES) $(INSTALL_DIR)
	install ../misc/gdb-macros $(INSTALL_DIR)

clean: 
	rm -f *.o setitimer-helper squish-pty squish-unix
