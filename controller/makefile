# makefile
CC=gcc
CFLAGS=-c -g -Wall
LDFLAGS=
LIBS=-lm
OBJECTS=$(SOURCES:.c=.o)
EXECUTABLE=controller.exe

SOURCES=controller.c discover.c

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@ $(LIBS)

.c.o:
	$(CC) $(CFLAGS) $< -o $@

clean:
	rm $(OBJECTS) $(EXECUTABLE)
