# Pequeña lista de comandos Git (usando Markdown 🙃)

En este documento Markdown voy a contar voy a enumerar algunos comandos de Git.

## Pasos para crear un repositorio de Git

![Imagen de git](https://i.blogs.es/672fa7/git-logo/450_1000.png)

* git init
* git add . (o git add archivo.txt)
* git commit m- 'Agregar un mensaje sobre el commit'
* git config --list: muestra la configuración del repositorio.
* git show archivo.txt: muestra los cambios de un archivo, y hace una comparación entre los cambios.
* git diff 'codigo viejo 'codigo reciente': hace una camparativa entre esos 2 commits, los cambios entre cada uno.
git diff: es para ver todos los cambios, trae los 'trae los codigo hexadecimales de los cambios'
* git reset 'codigo hexadecimal' -hard/soft: para volver a una versión anterior. Con -hard se pierden todos los commits hechos hasta ese punto. Con -soft se mantienen los cambios en el staging, se les pueden volver a hacer commit.
* git checkout 'codigo hexadecimal' 'archivo.txt': trae una version vieja a la versión actual.
* git checkout master 'archivo.txt': trae el master.
