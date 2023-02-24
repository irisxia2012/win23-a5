objects = main.o addition.o subtraction.o multiplication.o division.o
all: calculator
calculator: $(objects) operations.h
	cc -o calculator $(objects) operations.h
$(objects): %.o:%.c
	cc -c $< -o $@
clean:
	rm -f calculator $(objects)
.PHONY: clean
