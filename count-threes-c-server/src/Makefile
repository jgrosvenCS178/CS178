
SHELL = /bin/sh

objects = ServerCountThrees.o readInt32BitLE.o

test : $(objects)
	cc -o test $(objects)
	mkdir ../build/
	cp ../data/threesData.bin ../build
	cp test ../build

readInt32BitLE.o : readInt32BitLE.c 
	cc -c readInt32BitLE.c -o readInt32BitLE.o

ServerCountThrees.o : ServerCountThrees.c
	cc -c ServerCountThrees.c -o ServerCountThrees.o

ServerCountThrees : $(objects)
	cc -o ServerCountThrees $(objects)

.PHONY : clean
clean :
	-rm $(objects)
