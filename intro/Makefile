include ../Make.defines

PROGS = daytimetcpcli daytimetcpsrv

all: ${PROGS}

daytimetcpcli: daytimetcpcli.o
	$(CC) ${CFLAGS} -o $@ daytimetcpcli.o ${LIBS}

daytimetcpsrv: daytimetcpsrv.o
	$(CC) ${CFLAGS} -o $@ daytimetcpsrv.o ${LIBS}

daytimetcpcli_debug: clean
	$(CC) ${CFLAGS} daytimetcpcli.c -o daytimetcpcli ${LIBS}

daytimetcpsrv_debug: clean
	$(CC) ${CFLAGS} daytimetcpsrv.c -o daytimetcpsrv ${LIBS}

.PHONY: clean

clean:
	rm -rf *.o ${PROGS} *.dSYM

