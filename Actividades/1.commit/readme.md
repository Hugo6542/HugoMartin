. Compromisos
Para el primer ejercicio, se debe crear un archivo nombre_apellido.txt, dentro de la carpeta 1.commit.

En este archivo, se va a guardar las respuestas teóricas y algunos resultados de los mismos.

##Ejercicio 1

1.1. Preguntas
¿Cómo se inicializa un repositorio local? (que comando se debe ejecutar?)
¿Cómo hago para que un directorio deje de ser controlado por git? (que comando se debe ejecutar?)
Si agrega un archivo a un directorio que ya está siendo controlado por git, ¿está siendo controlado por git?
¿Qué comando se utiliza para agregar un archivo al repositorio local?
¿Cómo determina que archivos fueron modificados? (que comando se debe ejecutar?)
¿Qué comando se utiliza para hacer un commit?
En sus propias palabras, ¿qué es un compromiso?
1.2. Ejercicio práctico
Cree un archivo nombre_apellido.txtsi no estaba creado previamente.
Agrega sandwich.txtcondimentos e ingredientes que le gusten, simulando que es un sándwich que se va a comer.
Antes de realizar cualquier acción con git, guarde el estado actual del directorio en el archivo nombre_apellido.txt. Para esto, se debe ejecutar el comando git statusy copiar el resultado en el archivo nombre_apellido.txt. Explique que significa la salida del comando.
Agregar el archivo sandwich.txtal repositorio local. Para esto, se debe ejecutar el comando git add sandwich.txt.
Explique que cambio en la salida del comando git statusluego de ejecutar el comando git add sandwich.txt.
Realizar un commit con el mensaje "Agrego mi sandwich.txt". Para esto, se debe ejecutar el comando git commit -m "Agrego mi sandwich.txt".
Explique que cambio en la salida del comando git statusluego de ejecutar el comando git commit -m "Agrego mi sandwich.txt".
Agregar salsas de su preferencia a sandwich.txty realizar un commit con el mensaje "Agrego salsas".
Escriba la salida del comando git logen el archivo nombre_apellido.txt. Y explique que significa. ¿En qué orden aparecen los commits?
Pruebe las variaciones del comando git logy explique que observa en cada una de ellas. 10.1. git log --oneline 10.2.git log --stat
Inspeccione diferencias entre los commits, use el comando git diff y explique que significa cada uno de los resultados. 11.1. En Windows, pruebe git difftool --tool=meld <hash> 11.2. En Linux, pruebagit difftool --tool=opendiff <hash>
Cree un nuevo archivo dentro de la carpeta 1.commit, llamado sandwich2.txt, y agreguele los ingredientes de su sándwich.
Agregar el archivo sandwich2.txtal repositorio local.
Renombrar el archivo sandwich2.txta sandwich2_feo.txt. Para esto, se debe ejecutar el comando git mv sandwich2.txt sandwich2_feo.txt. Explique que cambio en la salida del comando git statusluego de hacer un commit con esos cambios y de git log --oneline.
Borre el archivo sandwich2_feo.txt. Para esto, se debe ejecutar el comando git rm sandwich2_feo.txt. Explique que cambio en la salida del comando git statusluego de hacer un commit con esos cambios y de git log --oneline.
Inspeccione la bitácora usando git log --staty explique lo que ve.
Finalizado
Una vez finalizado el ejercicio, recuerde guardar sus cambios en nombre_apellido.txty subirlos a su repositorio remoto. Este archivo ( README.md) y sandwitch.txttienen que mantenerse sin ningún cambio.

Para volver a sandwich.txtsu estado original, debe buscar el commit que lo contiene y correr el comando:

git checkout [commit ID] -- 1.commit/sandwich.txt

# ó

git checkout [commit ID] -- sandwich.txt

# dependiendo de donde esté ubicado
