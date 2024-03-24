src := writer.c
exec := writer

ifeq ($(CROSS_COMPILE),aarch64-none-linux-gnu-)
	CC := aarch64-none-linux-gnu-gcc
else
	CC := gcc
endif

writer: $(src)
	$(info Compiler selected is $(CC))
	$(CC) -o $(exec) $(src)

clean:
	rm -f $(exec)
