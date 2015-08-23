# Github

## Subir un proyecto a github

Primero hay que crear un nuevo repositorio en github
Luego, desde la carpeta del proyecto hacemos lo siguiente
	$ git remote add origin https://github.com/xabier/project1.git
se añade un origen "origin" que es la url del repositorio en github
luego escribimos
	$ git push -u origin master
con esto subimos los contenidos del repositorio local (master) al de github (origin)

## Comenzar de cero con un proyecto de github y descargarlo a tu directorio local

Al hacer los siguiente en la línea de comando se creará la carpeta correspondiente:
	$ git clone https://github.com/xabier/escritura-colaborativa-github.git

## Forkear repositorio

Visitamos un repositorio de github cualquier y pinchamos sobre el icono de fork, una vez hecho esto nos crea en nuestra cuenta una copia de todo el repositorio, copiamos la url (de nuestro fork en github).
Ahora podemos ya importarlo en local
	$ git clone https://github.com/xabier/first-repo

Ya tenemos el clon, pero vamos a crear una nueva rama (branch) de desarrollo y a decirle a git que nos movemos a esa rama
	$ git branch nombre-rama-nueva
	$ git checkout nombre-rama-nueva

Añadimos un nuevo documento y hacemos un commit 
	$ echo "testing" > testing.txt
	$ git add testing.txt 
	$ git commit -m "probando"

Ahora podemos actualizar ya la nueva rama
	$ git push -u origin nombre-rama-nueva

Crearemos ramas para cada cambio significativo y haremos un push cada vez para que se actualice en github

Solicitar un pull request (una petición de aceptar nuestros cambios en el repositorio original)

