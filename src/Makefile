# 11jan09abu
# (c) Software Lab. Alexander Burger

.SILENT:

CC=c:/Progra~2/LLVM/bin/clang.exe
bin = ../bin
picoFiles = main.c gc.c apply.c flow.c sym.c subr.c math.c io.c tab.c

picolisp: $(bin)/picolisp

.c.o:
	echo $*.c:
	$(CC) -w -c $*.c

$(picoFiles:.c=.o): pico.h

$(bin)/picolisp: $(picoFiles:.c=.o)
	c:/Progra~2/LLVM/bin/clang.exe -o picolisp $(picoFiles:.c=.o)
#	strip $(bin)/picolisp


# Clean up
clean:
	rm -f *.o

# vi:noet:ts=4:sw=4
