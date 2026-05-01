# ==========================================
# Name    : Abhi
# Project : Inverted Search Engine
# Purpose : Build and manage compilation
# ==========================================

CC = gcc
CFLAGS = -Wall

OBJ = main.o create_database.o display.o save_database.o search.o update.o

# Final executable
inverted_search : $(OBJ)
	$(CC) $(OBJ) -o inverted_search

# Object file rules
main.o : main.c inverted_search.h
	$(CC) $(CFLAGS) -c main.c

create_database.o : create_database.c inverted_search.h
	$(CC) $(CFLAGS) -c create_database.c

display.o : display.c inverted_search.h
	$(CC) $(CFLAGS) -c display.c

save_database.o : save_database.c inverted_search.h
	$(CC) $(CFLAGS) -c save_database.c

search.o : search.c inverted_search.h
	$(CC) $(CFLAGS) -c search.c

update.o : update.c inverted_search.h
	$(CC) $(CFLAGS) -c update.c

# Clean rule
clean :
	rm -f *.o inverted_search