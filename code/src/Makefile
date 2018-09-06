CC = gcc


TARGET = main


SRCS = $(wildcard *.c)
OBJS = $(patsubst %.c,%.o,$(SRCS))


$(TARGET):$(OBJS)
	$(CC) $(OBJS) -o $(TARGET) -lpthread

$(OBJS):%.o:%.c
	$(CC) -c $^ -o $@ -lpthread


clean:
	rm *.o 

