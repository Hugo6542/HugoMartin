# 2.1 Preguntas
**1 ¿Qué es una sucursal?**

Una rama que permite trabajar en cambios sin afectar el proyecto principal.

**2 ¿Por qué pueden ser útiles las sucursales?**

Permiten desarrollar y probar sin afectar el código principal.

**3 ¿Cómo se crea una rama?*

git branch nombre-de-la-rama

**4 ¿Cómo se cambia a una sucursal?*

git checkout nombre-de-la-rama

**5 ¿Cómo se elimina una rama?**

git branch -d nombre-de-la-rama

**6 ¿Cómo se crea una rama y se cambia a ella en un solo paso?**

git checkout -b nombre-de-la-rama

*7 ¿Qué es una merge?**

Unir los cambios de una rama con otra.

*8 ¿Cómo se realiza una fusión?**

git checkout main
git merge nombre-de-la-rama

**9 ¿Que es una etiqueta?**

Marca un commit importante (como una versión).

**10.Como se crea un tag**

git tag nombre-del-tag


##2.2. Ejercicio práctico

1-Crear una rama experimento. (Puede usar el comando

C:\Users\Usuario\IESlaCa-uelaAWEB>git branch experimento

2-Muévete a la rama experimento. (Puede usar el comando git checkout).

C:\Users\Usuario\IESlaCa-uelaAWEB>git checkout experimento
Switched to branch 'experimento'

3. Verifique que se encuentra en la sucursal ejercicio_2. (Puede usar el comando git branch).

   C:\Users\Usuario\IESlaCa-uelaAWEB>git branch
* experimento
  main
  rama-local

  4.Agregarle el condimento albahaca arriba del queso al archivo 2.branchs/pizza.txty "commitee" los cambios.

 C:\Users\Usuario\IESlaCa-uelaAWEB>git add Actividades/2.branchs/pizza.txt

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "he añadido el ingrediente Albahaca"

  5. Agregarle el condimento oregano arriba de la albahaca al archivo 2.branchs/pizza.txty "commitee" los cambios.
 
    C:\Users\Usuario\IESlaCa-uelaAWEB>git add Actividades/2.branchs/pizza.txt

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "He añadido oregano a la pizza"

     6. Correr el comando git graphy observar el resultado. ¿Qué observa?ç

     
C:\Users\Usuario\IESlaCa-uelaAWEB>git graph
* f6d0240 (HEAD -> experimento) he añadido el ingrediente Albahaca
* af8f154 He añadido oregano a la pizza

  7. Vuelva a la rama master.
 
  C:\Users\Usuario\IESlaCa-uelaAWEB>git checkout main

  8. Crear una sucursal anana. (Puede usar el comando git checkout -b anana).
 
C:\Users\Usuario\IESlaCa-uelaAWEB>git checkout -b anana
Switched to a new branch 'anana'

9. Agregarle el condimento anana debajo del queso al archivo 2.branchs/pizza.txty "comité" los cambios.

    C:\Users\Usuario\IESlaCa-uelaAWEB>git add Actividades/2.branchs/pizza.txt

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "He agregado el contimento anana"
[anana 66a159e] He agregado el contimento anana
 1 file changed, 3 insertions(+)

 10. Correr el comando git graph y observar el resultado. ¿Qué observa?

     C:\Users\Usuario\IESlaCa-uelaAWEB>git graph
* 66a159e (HEAD -> anana) He agregado el contimento anana
| * f6d0240 (experimento) He añadido oregano a la pizza
| * af8f154 he añadido el ingrediente oregano

11.Vuelva a la rama master.

C:\Users\Usuario\IESlaCa-uelaAWEB>git checkout main
Switched to branch 'main'


12. Agregue el condimento cebolla debajo de la salsa al archivo 2.branchs/pizza.txty "comité" los cambios.

    C:\Users\Usuario\IESlaCa-uelaAWEB>git add Actividades/2.branchs/pizza.txt

C:\Users\Usuario\IESlaCa-uelaAWEB>git commit -m "He añadido cebolla a la pizza"
[main 3ac067b] He añadido cebolla a la pizza
 1 file changed, 4 insertions(+)

 13. Correr el comando git graphy observar el resultado. ¿Qué observa?

     C:\Users\Usuario\IESlaCa-uelaAWEB>git graph
* 3ac067b (HEAD -> main) He añadido cebolla a la pizza
| * 66a159e (anana) He agregado el contimento anana
|/
| * f6d0240 (experimento) He añadido oregano a la pizza
| * af8f154 he añadido el ingrediente oregano
|/
 
14. Haga un merge de la rama ananaa la rama master.

    C:\Users\Usuario\IESlaCa-uelaAWEB>git graph
*   fd6938c (HEAD -> main) hago un mergue con la rama anana
|\
| * 66a159e (anana) He agregado el contimento anana
* | 3ac067b He añadido cebolla a la pizza
|/
| * f6d0240 (experimento) He añadido oregano a la pizza
| * af8f154 he añadido el ingrediente oregano
|/        

  
   

