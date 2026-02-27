En el experimento se observ¢ que pasar estructuras grandes por valor implica copiar completamente la estructura en cada llamada, generando un alto costo de tiempo debido al movimiento masivo de memoria.
En contraste, al pasar la estructura por referencia, solo se copia la direcci¢n de memoria, reduciendo dr sticamente el tiempo de ejecuci¢n.
Los resultados mostraron que el paso por puntero fue aproximadamente 1400 veces m s r pido, demostrando la importancia de evitar copias innecesarias en sistemas de alto rendimiento.
