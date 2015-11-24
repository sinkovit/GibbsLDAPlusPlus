CC=		g++
CFLAGS=         -O3

OBJS=		strtokenizer.o dataset.o utils.o model.o
MAIN=		lda

all:	$(OBJS) $(MAIN).cpp
	$(CC) $(CFLAFGS) -o $(MAIN) $(MAIN).cpp $(OBJS)
	strip $(MAIN)

strtokenizer.o:	strtokenizer.h strtokenizer.cpp
	$(CC) $(CFLAFGS) -c -o strtokenizer.o strtokenizer.cpp

dataset.o:	dataset.h dataset.cpp
	$(CC) $(CFLAFGS) -c -o dataset.o dataset.cpp

utils.o:	utils.h utils.cpp
	$(CC) $(CFLAFGS) -c -o utils.o utils.cpp

model.o:	model.h model.cpp
	$(CC) $(CFLAFGS) -c -o model.o model.cpp

test:

clean:
	rm $(OBJS)
	rm $(MAIN)

