SOURCES = harvest.lua \
	cliargs.lua cliargs/*.lua cliargs/utils/*.lua \
	align.lua

all:
	$(CC) -c $(INCLUDE) $(CFLAGS) lfs.c -o lfs.o
	$(AR) rcs lfs.a lfs.o
	CC="" luastatic $(SOURCES) lfs.a
	$(CC) -c $(INCLUDE) $(CFLAGS) harvest.lua.c
