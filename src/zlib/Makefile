


.PHONY : all

.PHONY : clean



all: adler32.o compress.o crc32.o deflate.o gzclose.o gzlib.o gzread.o gzwrite.o infback.o inffast.o inflate.o inftrees.o trees.o uncompr.o zutil.o
	$(CC) $(CFLAGS) -shared -o zlib.so adler32.o compress.o crc32.o deflate.o gzclose.o gzlib.o gzread.o gzwrite.o infback.o inffast.o inflate.o inftrees.o trees.o uncompr.o zutil.o

%.o: %.c
	$(CC) $(CFLAGS) -c -fPIC -o $@ $^


clean:
	$(RM) adler32.o compress.o crc32.o deflate.o gzclose.o gzlib.o gzread.o gzwrite.o infback.o inffast.o inflate.o inftrees.o trees.o uncompr.o zutil.o
	$(RM) zlib.so
