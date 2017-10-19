SHELL = /bin/sh

objects = ServerCountThrees.o readInt32BitLE.o

test : $(objects)
	cc -o test $(objects)
	mkdir build
	cp ../data/threesData.bin /src/build	
	cp test ./build

ServerCountThrees : $(objects)
	cc -o ServerCountThrees $(objects)

ServerCountThrees.o : ServerCountThrees.c
	cc -o -c ServerCountThrees.c

readInt32BitLE.o : readInt32BitLE.c readInt32BitLE.h
	cc -c readInt32BitLE.c


.PHONY : clean
clean :
	-rm ServerCountThrees $(objects)
