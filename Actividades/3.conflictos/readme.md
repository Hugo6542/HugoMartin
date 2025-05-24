. Conflictos
Para este ejercicio, se debe crear un archivo nombre_apellido.txt, dentro de la carpeta 1.commit.

En este archivo, se va a guardar las respuestas teóricas y algunos resultados de los mismos.

Ejercicio 3
3.1. Preguntas
¿Qué es un conflicto? ¿Cuándo ocurre? ¿Es bueno o malo?
¿Se puede evitar un conflicto? ¿Cómo?
3.2. Ejercicio práctico
Cree un archivo nombre_apellido.txtdentro de la carpeta 3.conflicts.
Crear una nueva sucursal supremaa partir de la sucursal master. (Puede usar el comando git checkout -b suprema).
Muévete a la rama suprema. (Puede usar el comando git checkout).
Cambiar el contenido del archivo 3.conflicts/milanesa.txtdonde dice lomo por pollo.
"Comité" los cambios. (Puede usar el comando git commit -am "Cambio de lomo a pollo").
Muévete a la rama master. (Puede usar el comando git checkout).
Crear una nueva sucursal bifea partir de la sucursal master. (Puede usar el comando git checkout -b bife).
Muévete a la rama bife. (Puede usar el comando git checkout).
Cambiar el contenido del archivo 3.conflicts/milanesa.txtdonde dice lomo por bife.
Haga un git diff master supremay un git diff master bife. ¿Qué observa?
Muévete a la rama master. Corra un git status, ¿qué observa?
Ejecutar git merge bife. ¿Funcionó?
Ejecutar git merge suprema. ¿Funcionó?
Ejecutar git status. ¿Que observa?
Vea el contenido del archivo 3.conflicts/milanesa.txt. ¿Qué observa?
Cancelar la fusión. (Puede usar el comando git merge --abort).
Vuelva a ejecutar git merge suprema.
Resuelva el conflicto manualmente.
Finalizado
Una vez finalizado el ejercicio, recuerde guardar sus cambios en nombre_apellido.txty subirlos a su repositorio remoto. Este archivo ( README.md) y milanesa.txttienen que mantenerse sin ningún cambio.

Para volver a milanesa.txtsu estado original, debe buscar el commit que lo contiene y correr el comando:

git checkout [commit ID] -- 3.conflicts/milanesa.txt

# ó

git checkout [commit ID] -- milanesa.txt

# dependiendo de donde esté ubicado
