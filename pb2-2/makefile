

LINK_TARGET = main

OBJS = \
	main.o \
	advent.o

REBUILDABLES = $(OBJS) $(LINK_TARGET)

all : $(LINK_TARGET)

clean: 
	rm -f $(REBUILDABLES)

$(LINK_TARGET) : $(OBJS)
	cc -g -o $@ $^ 
	
%.o : %.c
	cc -g  -Wall -o $@ -c $<
  
main.o: advent.h advent.c