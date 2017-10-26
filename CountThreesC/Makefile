# Name: Justin Grosvenor
# Course: CS178 Build Automation for DevOps and QA
# CRN: 76718
# Date: 8/30/2017
# Assignment: Makefile
# --------------------------------------------------
SHELL = /bin/sh

objects = countThrees.o readInt32BitLE.o
all = countThrees.c readInt32BitLE.c readInt32BitLE.h

Count3s : $(objects)
	cc $(objects) -o Count3s

readInt32BitLE.o : readInt32BitLE.c readInt32BitLE.h
	cc -c readInt32BitLE.c -o readInt32BitLE.o

countThrees.o : countThrees.c
	cc -c countThrees.c -o countThrees.o

runCountThrees : $(objects)
	cc $(objects) -o runCountThrees
	./runCountThrees

.PHONY : clean
clean :
	-rm $(objects)
