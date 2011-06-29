CC=g++
CFLAGS=-c -Wall
ARCH=-arch i386

all: testcpp sgp4io sgp4unit sgp4ext
	$(CC) $(ARCH) sgp4io.o sgp4unit.o sgp4ext.o testcpp.o -o sgp4

testcpp: testcpp.cpp
	$(CC) $(CFLAGS) $(ARCH) testcpp.cpp
    
sgp4io: sgp4io.cpp sgp4io.h
	$(CC) $(CFLAGS) $(ARCH) sgp4io.cpp

sgp4unit: sgp4unit.cpp sgp4unit.h
	$(CC) $(CFLAGS) $(ARCH) sgp4unit.cpp

sgp4ext: sgp4ext.cpp sgp4ext.h
	$(CC) $(CFLAGS) $(ARCH) sgp4ext.cpp

clean:
	rm -rf *.o sgp4
