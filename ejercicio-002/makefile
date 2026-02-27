TARGET = experimento
LOG_FILE = registro_valgrind.txt

all:
	gcc -g ejercicio-002.c -o $(TARGET)

valgrind: all
	valgrind --leak-check=full --log-file=$(LOG_FILE) ./$(TARGET)
	@echo "An lisis completado. Revisa $(LOG_FILE)"

