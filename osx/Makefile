CFLAGS	:= -O3 -std=c++14

CC = g++ 
SRC := ../src
OBJS := objmemory.o bitblt.o main.o interpreter.o

Smalltalk: $(OBJS) 
	$(CC) -F/Library/Frameworks -framework SDL2  -o $@  $^
	
main.o: $(SRC)/main.cpp
	$(CC) $(CFLAGS) -I/Library/Frameworks/SDL2.framework/Headers -F/Library/Frameworks   -c $(SRC)/main.cpp

%.o: $(SRC)/%.cpp
	$(CC) $(CFLAGS) -c $<  -o $@


clean:
	rm -f *.o Smalltalk

