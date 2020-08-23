include ../Make.defines

PROGS = daytimetcpcli

all: ${PROGS}

daytimetcpcli: daytimetcpcli.o
	$(CC) ${CFLAGS} -o $@ daytimetcpcli.o ${LIBS}

%.o: %.c
	$(CC) -c $^ -o $@

.PHONY: clean

clean:
	rm -rf *.o


