##3 Conflictos
Para este ejercicio, se debe crear un archivo nombre_apellido.txt, dentro de la carpeta 1.commit.

En este archivo, se va a guardar las respuestas teóricas y algunos resultados de los mismos.

Ejercicio 3
3.1. Preguntas
1. ¿Qué es un conflicto? ¿Cuándo ocurre? ¿Es bueno o malo?

Qué es un conflicto en Git?
Es cuando Git no puede combinar cambios porque dos ramas modificaron las mismas líneas de un archivo.

¿Cuándo ocurre?
Durante un merge, rebase u operación similar con cambios que se solapan.

¿Es bueno o malo?
No es malo. Es normal y necesario resolverlo manualmente para decidir qué cambios conservar.

2. ¿Se puede evitar un conflicto? ¿Cómo?

   ¿Se puede evitar un conflicto?
Sí.

¿Cómo?

Haciendo pull y merge frecuentemente.

Comunicándose con el equipo.

Editando archivos diferentes o partes distintas del mismo archivo.

3.2. Ejercicio práctico

2. Crear una nueva sucursal supremaa partir de la sucursal master. (Puede usar el comando git checkout -b suprema).

   C:\Users\Usuario\HugoMartin>git checkout -b suprema
Switched to a new branch 'suprema'

3. Muévete a la rama suprema. (Puede usar el comando git checkout).

   

