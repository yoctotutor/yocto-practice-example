#export CC=gcc
#export LDFLAGS =-Wall -Werror -fpic

libhello.so:
	${CC}  -c ${LDFLAGS} foo.c
	${CC} -shared -o libfoo.so.1 foo.o

clean:
	rm -rf *.so* *.o
