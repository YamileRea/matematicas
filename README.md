# matematicas


## Manual
Hola compañer@

Este txt fue hecho para recordar rápido el proceso para trabajar con git asumiendo que ya tienes configurado git y se pudo clonar el repo de forma correcta y tienen los permisos para trabajar con él.

1. No agregar código a nada del main
2. Para trabajar crea una nueva rama del repositorio con git branch
	Ejemplo: Añadir el ejercicio 5
		Escribe:
			`git branch ej5`
		(puede ser el nombre que sea pero you know... nombres autoexplicativos y eso)
		Luego para moverte a tu rama escribe:
			`git checkout ej5`
		Nota. si no sabes en que rama estás solo escribe "`git branch`" y te dará una lista de las ramas disponibles donde una tendrá un "*" que indica en cual estás trabajando pero si tu terminal está bien configurada normalmente te lo indica arriba.
3. Una vez en tu nueva y flamante rama ya puedes editar lo que necesites, ya sea un archivo de haskell, .tex, o lo que sea, puedes usar el editor que quieras eso es lo de menos la vdd.
4. Checa que todo jala, compila o se interpreta de forma correcta.
5. Borra los archivos basura que puedan generarse, latex por ejemplo al compilarse arroja archivos .aux, .log y .pdf (si, también borra el pdf porque ese lo podemos hacer nosotros)
6. Agrega los archivos que utilizaste al area de staging (lo que le indica a git donde están los cambios)
7. utiliza
	`git status`
	Esto debería mostrar los archivos que van a guardarse en el commit y solo debería ser el .hs y el .tex (en nuestro caso)
8. Si vas a agregar una imagen, hay una carpeta para eso, dejala ahí y con el "`git add .`" también se subirá.
9. Haz tu commit :3, eso ya lo sabes de ICC
10. Ve a la rama principal con
	`git checkout main`
11. IMPORTANTE, antes de juntar las ramas, en el caso de que alguien mientras tanto haya subido algo debemos anticiparnos a eso y escribir:
	`git pull`
	Esto atraerá los últimos cambios del repo
12. Ahora si juntamos nuestras ramas
		`git merge ej5`
		Obvio cambian "ej5" por el nombre de su rama jaja
13. Si todo salió bien no habrá problemas y pueden hacer lo mismo de ICC
	`git push`

Y ya, es todo, en caso de que alguien haya modificado algo de código con el que estabas trabajando tendrás un "conflicto", la vdd esperemos no lleguemos a eso pero cualquier cosa ahí se arregla xd
	

