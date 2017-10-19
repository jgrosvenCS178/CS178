
SHELL = /bin/sh

objects = ServerCountThrees.o readInt32BitLE.o

test : $(objects)
	cc -o test $(objects)
	mkdir ../build/
	cp ../data/threesData.bin ../build
	cp test ../build

readInt32BitLE.o : readInt32BitLE.c readInt32BitLE.h
	cc -c readInt32BitLE.c

ServerCountThrees.o : ServerCountThrees.c
	cc -o -c ServerCountThrees.c

ServerCountThrees : $(objects)
	cc -o ServerCountThrees $(objects)

.PHONY : clean
clean :
	-rm $(objects)
