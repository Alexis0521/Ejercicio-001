TARGET = experimento3
SRC = main.c
LOG = resultado.txt

all:
	gcc -std=c11 $(SRC) -o $(TARGET)

run: all
	./$(TARGET)

txt: all
	./$(TARGET) > $(LOG)

clean:
	rm -f $(TARGET) $(LOG)
