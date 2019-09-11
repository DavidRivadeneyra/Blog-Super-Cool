# Pequeña lista de comandos Git (usando Markdown 🙃)

En este documento Markdown voy a enumerar algunos comandos de Git.

## Pasos para crear un repositorio de [Git]

![Imagen de git][ImgenGit]

* **git init**
* **git add .** (o git add archivo.txt)
* **git commit m- 'Agregar un mensaje sobre el commit'**
* **git config --list**: muestra la configuración del repositorio.
* **git show archivo.txt**: muestra los cambios de un archivo, y hace una comparación entre los cambios.
* **git diff 'codigo viejo 'codigo reciente'**: hace una camparativa entre esos 2 commits, los cambios entre cada uno.
* **git diff**: es para ver todos los cambios, trae los 'trae los codigo hexadecimales de los cambios'
* **git reset 'codigo hexadecimal' -hard/soft**: para volver a una versión anterior. Con -hard se pierden todos los commits hechos hasta ese punto. Con -soft se mantienen los cambios en el staging, se les pueden volver a hacer commit.
* **git checkout 'codigo hexadecimal' 'archivo.txt'**: trae una version vieja a la versión actual.
* **git checkout master 'archivo.txt'**: trae el master.

## Comandos nuevos

1. **git remote add origin https://github.com/DavidRivadeneyra/Blog-Super-Cool.git**: Agregar origen remoto a mi repositorio.
2. **git remote >**: devuelve origin.
3. **git remote -v >**: devuelve que ya estoy habilitado en hacer origin  https://github.com/DavidRivadeneyra/Blog-Super-Cool.git (fetch) y origin  https://github.com/DavidRivadeneyra/Blog-Super-Cool.git (push).
4. **git push origin master**: enviar al origen (https://github.com/DavidRivadeneyra/Blog-Super-Cool.git) la rama master.
5. Sin ocurre un error porque no se han conectado anteriormente el master del Github y Git de mi máquina local.
6. **git pull orgin master**: es la combinación de git fetch y git merge.
7. Devuelve una advertencia, porque no hay commits comunes, la historia entre Github es diferente de Git (local). 
8. **git pull origin master --allow-unrelated-histories**: permite fusionar a rama de Github con mi local, así permite hacer el merge con la rama maste de guthub.
9. **git push origin master**: para enviar mi repositorio local a Github.
10. **blame**: es para revisar quien hizo los cambios en github.
11. Se puede editar desde Github.
12. Luego en mi git local hago un **git pull origin master**, los cambios de Github se reflejan en mi git local.
13. Cool!!!!


[Git]:https://git-scm.com/
[ImgenGit]:https://git-scm.com/images/logo@2x.png