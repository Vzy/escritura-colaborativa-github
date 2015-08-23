
# Git basics

Seguimos el manual
http://git-scm.com
Y el tutorial https://www.youtube.com/watch?v=U8GBXvdmHT4

Instalar

 	$ sudo apt-get install git

Configurar tu identidad en git

 	$ git config --global user.name "tunombre"
 	$ git config --global user.email "tu@email.com"

Crear repositorio local nuevo

	$ git init proyecto1 

crea la carpeta proyecto1/ con un .git/ dentro que tiene el repositorio, config, etc.

Alternativamente, si ya tienes una carpeta con un proyecto, simplemente se entra en la carpeta y 

 	$ git init

Comprobar el estado del repositorio

 	$ git status

Añadir un archivo para que se actualice el repositorio

 	$ echo "lalala" > uno.txt

creamos así un archivo

 	$ git add uno.txt

así añadimos uno.txt al repositorio

 	$ git add . 

así añadimos todo lo que hay nuevo

Registrar cambios o actualizar el repositorio

 	$ git commit -m "comentario"

Voler a actualizar

 	$ git add .
 	$ git commit -m "otro comentario"

NOTA: hay que hacer el git add siempre :(
