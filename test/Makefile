TARGET	= test
SRCS	= testmain.cpp\
				dummytest.cpp

OBJS	= testmain.o\
				dummytest.o

CC = g++
LIBS =-L/usr/local/lib -ldl -lm -lstdc++ -lpthread -lcppunit  
INCLUDES=-I/usr/local/include

CFLAGS= -std=c++0x -g -O0
all: $(TARGET)

$(TARGET): $(OBJS) $(SRCS)
	$(CC) $(CFLAGS) -o $@ $(OBJS) $(LIBS)




.cpp.o:
	$(CC) $(CFLAGS) -c -o $@ $<

clean:
	rm -f $(OBJS) $(TARGET)
