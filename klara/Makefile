SRCS	= matmult_nmk.c matmult_nkm.c matmult_mnk.c matmult_mkn.c matmult_knm.c matmult_kmn.c
OBJS	= $(SRCS:.c=.o)
TARGET	= libmatmult.so
CC	= gcc -std=c99 -fPIE
INCS	= 
DBG	= -g 
OPT	= -O3 
PARA	= 
CFLAGS	= $(DBG) $(OPT) $(PARA) $(XOPTS)

$(TARGET): $(OBJS)  #let's link library files into a static library
	$(CC) *.o -shared -o $(TARGET)

clean:
	rm -f *.o *.so 
