# ✨ Cómo compilar y ejecutar el programa

## Usando el **Makefile** 🛠️  
#¡Es fácil! Simplemente abre tu terminal y ejecuta:  
make

#Compilación manual 📝
##Si prefieres hacerlo paso a paso, sigue estas instrucciones:

# 1. Compila el scanner 
flex scanner.l

# 2. Compila el parser 
bison -d parser.y

# 3. Junta todos los archivos .c en un ejecutable
gcc -Wall -g *.c -lfl

# 4. Ejecuta el programa 
./a.out < enunciado/entrada.txt > enunciado/salida.txt

#✨ Nota: Por defecto, el ejecutable se llamará a.out (ya está incluido en el .gitignore).
