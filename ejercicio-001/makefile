TARGET = mi_programa
LOG_FILE = registro_valgrind.txt

all:
	gcc -g main.c -o $(TARGET)

valgrind: all
	valgrind --leak-check=full --log-file=$(LOG_FILE) ./$(TARGET)
	@echo "Registro guardado en $(LOG_FILE)"
all: clean compilar
	
clean:
	rm -rf cache_demo a.out cachegrind.out.*

compilar:
	gcc -O2 -std=c11 cache_demo.c -o cache_demo

valgrindf: compilar
	valgrind --tool=cachegrind --cache-sim=yes --branch-sim=yes ./cache_demo f

valgrindc: compilar
	valgrind --tool=cachegrind --cache-sim=yes --branch-sim=yes ./cache_demo c
