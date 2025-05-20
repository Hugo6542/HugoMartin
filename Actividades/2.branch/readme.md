2. Ramas
Para este ejercicio, se debe crear un archivo nombre_apellido.txt, dentro de la carpeta 2.branchs.

En este archivo, se va a guardar las respuestas teóricas y algunos resultados de los mismos.

Ejercicio 2
2.1. Preguntas
¿Qué es una sucursal?
¿Por qué pueden ser útiles las sucursales?
¿Cómo se crea una rama?
¿Cómo se cambia a una sucursal?
¿Cómo se elimina una rama?
¿Cómo se crea una rama y se cambia a ella en un solo paso?
¿Qué es una merge?
¿Cómo se realiza una fusión?
¿Que es una etiqueta?
¿Cómo se crea una etiqueta?
2.2. Ejercicio práctico
Antes de continuar con el ejercicio, se debe agregar un alias para facilitar la visualización de las ramas.

git config --global alias.graph "log --all --graph --decorate --oneline"

# Pruebe el comando
git graph
[] Crear una rama experimento. (Puede usar el comando git branch experimento master).
Muévete a la rama experimento. (Puede usar el comando git checkout).
Verifique que se encuentra en la sucursal ejercicio_2. (Puede usar el comando git branch).
Agregarle el condimento albahaca arriba del queso al archivo 2.branchs/pizza.txty "commitee" los cambios.
Agregarle el condimento oregano arriba de la albahaca al archivo 2.branchs/pizza.txty "commitee" los cambios.
Correr el comando git graphy observar el resultado. ¿Qué observa?
Vuelva a la rama master.
Crear una sucursal anana. (Puede usar el comando git checkout -b anana).
Agregarle el condimento anana debajo del queso al archivo 2.branchs/pizza.txty "comité" los cambios.
Correr el comando git graphy observar el resultado. ¿Qué observa?
Vuelva a la rama master.
Agregue el condimento cebolla debajo de la salsa al archivo 2.branchs/pizza.txty "comité" los cambios.
Correr el comando git graphy observar el resultado. ¿Qué observa?
Haga un merge de la rama ananaa la rama master. (Puede usar el comando git merge anana).
Correr el comando git graphy observar el resultado. ¿Qué observa?
¿Qué sucursales están "fusionadas" con un maestro? (Puede usar el comando git branch --merged).
Haga un merge de la rama experimentoa la rama master. (Puede usar el comando git merge experimento).
Correr el comando git graphy observar el resultado. ¿Qué observa?
¿Tuvo que hacer un merge manual, o git lo hizo automáticamente? ¿Por qué?
¿Qué sucursales están "fusionadas" con un maestro? (Puede usar el comando git branch --merged).
Eliminar la rama anana. (Puede usar el comando git branch -d anana).
Eliminar la rama experimento. (Puede usar el comando git branch -d experimento).
¿Qué sucursales están "fusionadas" con un maestro? (Puede usar el comando git branch --merged).
Correr el comando git graphy observar el resultado. ¿Qué observa?
Crea una etiqueta pizzaen el último commit. (Puede usar el comando git tag -a pizza -m "Receta de la pizza."").
Ver las etiquetas creadas. (Puede usar el comando git tag).
Ver la etiqueta pizza. (Puede usar el comando git show pizza).
Finalizado
Una vez finalizado el ejercicio, recuerde guardar sus cambios en nombre_apellido.txty subirlos a su repositorio remoto. Este archivo ( README.md) y pizza.txttienen que mantenerse sin ningún cambio.

Para volver a sandwich.txtsu estado original, debe buscar el commit que lo contiene y correr el comando:

git checkout [commit ID] -- 2.branchs/pizza.txt

# ó

git checkout [commit ID] -- pizza.txt

# dependiendo de donde esté ubicado
