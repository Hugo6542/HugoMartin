#1.1. Preguntas


*1. ¿Cómo se inicializa un repositorio local? (que comando se debe ejecutar?)**

el comando git init

*2. ¿Cómo hago para que un directorio deje de ser controlado por git? (que comando se debe ejecutar?)**

el comando git ignore <Directorio>

*3. Si agrega un archivo a un directorio que ya está siendo controlado por git, ¿está siendo controlado por git?**

Si.

**4. ¿Qué comando se utiliza para agregar un archivo al repositorio local?**

El comando git add.

**5. ¿Cómo determina que archivos fueron modificados? (que comando se debe ejecutar?)**

El comando es git status

*6. ¿Qué comando se utiliza para hacer un commit?**

el comando es git commit -m "comentario de cambios"

**7. En sus propias palabras, ¿qué es un compromiso?**

Es un comando que confirma los combios que se han realizado

##1.2. Ejercicio práctico

**3.**
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   Actividades/1.commit/sandwich.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Actividades/1.commit/Hugo_Martin.md

no changes added to commit (use "git add" and/or "git commit -a")

Explique que significa la salida del comando.

Hay un archivo modificado y un archivo nuevo que hay que agregar y no hay nada listo para ser confirmado.

**5. Explique que cambio en la salida del comando git statusluego de ejecutar el comando git add sandwich.txt.**

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   Actividades/1.commit/sandwich.txt

El archio modficado ha sido agregado y no ha dado error

**7. Explique que cambio en la salida del comando git status luego de ejecutar el comando git commit -m "Agrego mi sandwich.txt".**

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "Agrego mi sandwich.txt"
[main 52e43f5] Agrego mi sandwich.txt
 1 file changed, 2 insertions(+), 1 deletion(-)

C:\Users\Usuario\IESlaCa-uelaAWEB>git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

El archivo se ha modificado y esta esperando al push para ser publicado

**8. Agregar salsas de su preferencia a sandwich.txty realizar un commit con el mensaje "Agrego salsas".**

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "Agrego salsas"
[main 2f1b269] Agrego salsas
 1 file changed, 1 insertion(+)

9. Escriba la salida del comando git logen el archivo nombre_apellido.txt. Y explique que significa. ¿En qué orden aparecen los commits?

git log muestra el hitorial de commit en un repositorio, el orden va del mas reciente al mas antiguo

10. Pruebe las variaciones del comando git logy explique que observa en cada una de ellas. 10.1. git log --oneline 10.2.git log --stat
git log --oneline muestra el historial de commits en una sola linea 
git log --stat muestra informacion estadistica sobre los cambios relaizados en cada commit


11. Inspeccione diferencias entre los commits, use el comando git diff y explique que significa cada uno de los resultados.

El comando difeencia la version antigua y actual de los commit 

14.Renombrar el archivo

Usando git status:

On branch main
Your branch is ahead of 'origin/main' by 3 commits.
  (use "git push" to publish your local commits)


El commit esta a la espera del push

usando el git log --oneline:
dba7954 (HEAD -> main) Agregacion de archivo sandwich2.txt y cambio de nombre a sandwich2_feo.txt


15. Borre el archivo sandwich2_feo.txt.

Usando el git status:

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        deleted:    Actividades/1.commit/sandwich2_feo.txt

Despues del commit:

Your branch is ahead of 'origin/main' by 4 commits.
  (use "git push" to publish your local commits)

usando el git log --oneline:

d75308f (HEAD -> main) Eliminacion de archivo sandwich2_feo.txt

16. nspeccione la bitácora usando git log --stat y explique lo que ve.

Aparecen todos los cambios y commit realizados.

