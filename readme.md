✨ Cómo compilar y ejecutar el programa
Usando el Makefile 🛠️
¡Es fácil! Simplemente abre tu terminal y ejecuta:

make
Compilación manual 📝
Si prefieres hacerlo paso a paso, sigue estas instrucciones:

Compila el scanner
Ejecuta el siguiente comando para procesar el archivo scanner.l:


flex scanner.l
Compila el parser
Procesa el archivo parser.y con este comando:


bison -d parser.y
Compila los archivos .c
Junta todos los archivos .c en un solo ejecutable con:


gcc -Wall -g *.c -lfl
✨ Nota: Por defecto, el ejecutable se llamará a.out (ya está incluido en el .gitignore).

Ejecuta el programa
Una vez compilado, puedes ejecutarlo con:


./a.out < enunciado/entrada.txt > enunciado/salida.txt
