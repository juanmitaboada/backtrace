# Make sure to have installed
apt-get install binutils-dev

# IBERTY
CC_FLAGS += -I/usr/include/libiberty
LD_FLAGS += -lbfd -liberty

# COMPILATION
$(CC) $(CC_FLAGS) -c $(DIRSRC)/backtrace-symbols.c -o $(DIROBJ)/backtrace-symbols.o

# LINKING
$(DIROBJ)/backtrace-symbols.o \
