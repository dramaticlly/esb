# Created Oct 2012
#
# By Evan Andersen 
#
# esb slave


OBJECTS = global.o main.o network.o slave.o tester.o

default: $(OBJECTS)
	gcc $(OBJECTS) -lcrypto -lm -lpthread  -g -Os -std=gnu99 -o esb-slave ../../src/libstorage.a libjansson.a -lcrypt

%.o : %.c
	gcc -std=gnu99 -c -O2 -g $<

clean:
	rm -rf $(OBJECTS)
	rm -rf esb-slave

