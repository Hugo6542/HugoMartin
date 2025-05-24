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

   C:\Users\Usuario\HugoMartin>git checkout suprema
Already on 'suprema'

C:\Users\Usuario\HugoMartin>git branch
  main
  rama-local
* suprema

5. "Comité" los cambios. (Puede usar el comando git commit -am "Cambio de lomo a pollo").
C:\Users\Usuario\HugoMartin>git commit -am "Cambio de lomo a pollo"
On branch suprema
nothing to commit, working tree clean

6. Muévete a la rama master. (Puede usar el comando git checkout).

   C:\Users\Usuario\HugoMartin>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

7. Crear una nueva sucursal bifea partir de la sucursal master. (Puede usar el comando git checkout -b bife).

   C:\Users\Usuario\HugoMartin>git checkout -b bife
Switched to a new branch 'bife'

8. Muévete a la rama bife. (Puede usar el comando git checkout).

   C:\Users\Usuario\HugoMartin>git checkout -b bife
Switched to a new branch 'bife'

C:\Users\Usuario\HugoMartin>git checkout bife
Already on 'bife'

10. Haga un git diff master supremay un git diff master bife. ¿Qué observa?

¿Qué observas?
Ambas ramas cambian la misma línea: lomo → pollo y lomo → bife.

Esto indica que habrá un conflicto al fusionar ambas.

11. Muévete a la rama master. Corra un git status, ¿qué observa?

    C:\Users\Usuario\HugoMartin>git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Main está limpio, sin cambios.

12. Ejecutar git merge bife. ¿Funcionó?

    Sí, porque master no cambió esa línea y bife sí → Git lo puede aplicar sin conflicto.

    13. Ejecutar git merge suprema. ¿Funcionó?
   
        No, aparece un conflicto, porque:

master ya tiene "bife".

suprema intenta poner "pollo" en la misma línea

14. Ejecutar git status. ¿Que observa?

    El archivo está en conflicto, con marcadores como: <<<<<<< HEAD
bife
=======
pollo
>>>>>>> suprema

15. Vea el contenido del archivo 3.conflicts/milanesa.txt. ¿Qué observa?
    

   

