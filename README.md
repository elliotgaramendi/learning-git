# AprendizajeGit
Aprendizaje de Git desde 0.
En este repositorio muestro como voy aprendiendo poco a poco los comandos de git bash, espero aprender mucho.

![alt text](https://miro.medium.com/max/352/1*qR6xp69TZSS9Dv_ZBxTw1w.jpeg)

## Comandos empleados en el aprendizaje
```
Brinda ayuda sobre los comandos

git [comandos]* help
```
### Repositorio local
```
Configura el email y usuario

git config --global user.email elliotgaramendi@gmail.com
git config --global user.name ElliotXLeo
```

```
Inicia un nuevo repositorio y crea la carpeta oculta .git

git init
```

```
Ver estado de los archivos no registrados

git status
```

```
Agregar todos los archivos pendientes de cambios

git add --all
```

```
Captura estado del código y lo almacena en el repositorio local posterior a la agregación de archivos

git commit -m "[descripción]"
```

```
Deshace la captura del estado del código

git reset
```

```
Abre editor de texto VIM del último commit realizado para poder modificar su nombre y vuelve a realizar el commit, también es útil para adicionar una modificación que se te olvidó en el último commit

git commit --amend
```

```
Muestra los commit realizados

git log --oneline
```

```
Lista todos los commits de forma gráfica

git log --oneline --graph
```

```
Lista todos los commits de todas las ramas de forma gráfica tomando como base la rama actual

git log --oneline --graph --all
```

```
Cambiamos a un commit en específico por su código. Ejemplo: f52f3da

git checkout f52f3da
```

```
Cambiamos a un commit en específico por su código con el objetivo de volver a empezar desde ese punto. Ejemplo: f52f3da

git reset --hard f52f3da
```

```
Crea una nueva rama

git branch nombreRama
```

```
Nos muestra en que rama estamos

git branch
```

```
Nos movemos de la rama actual a una específica

git checkout nombreRama
```

```
Eliminar una rama

git branch -d nombreRama
```

```
Cuando se trabaja en diferentes ramas y lo que busca es juntar dos de ellas para que tengan el mismo código. Se emplea el siguiente comando desde la rama principal invocando a la rama que se quiera unir a esta.

git merge nombreRama
```

```
Permite juntar dos ramas, pero mantiene la existencia de cada una de forma que se puede ver un gráfico de ramas.

git merge --no-ff develop
```

```
Crear un tag

git tag nombreTag -m "Versión alpha"
```

```
Listar tags

git tag
```

```
Borrar tags

git tag -d nombreTags
```

```
Hacer un tag en un commit anterior ej: f52f3da

git tag -a nombreTag f52f3da -m "Version alpha"
```

```
Mostrar información del tag

git show nombreTag
```

### Repositorio remoto
#### Para subir nuestro proyecto debemos crear un nuevo repositorio, al momento de la creación nos mostrará una serie de comandos para subir el proyecto.

```
Vincular repositorio remoto con repositorio de origen local y subir archivos del repositorio origen local al remoto

git remote add origin https://github.com/ElliotXLeo/AprendizajeGit.git
git push -u origin master

Al ejecutar estas líneas de comando te pedirá el usuario y contraseña de tu cuenta de github.
```

```
Nos muestra en que repositorio estamos enlazados remotamente.

git remote -v
```

```
Al ejecutar el comando git push estaremos subiendo todos los cambios locales al servidor remoto de GitHub, ten en cuenta que tienes que estar enlazado con tu repositorio remoto

git push
```

```
Subir los tags al repositorio remoto, por defecto si creaste un proyecto con diferentes versiones no subirá los tags, para eso tenemos el siguiente comando.

git push --tags
```

```
Hacer push a un repositorio remoto en otras ramas que no sea master

git push origin nombreRama
```

```
Cuando hay cambios en el repositorio remoto, es esencial realizar un pull, donde descargaremos los cambios realizados para seguir trabajando.

git pull
```

```
Este comando hace la comparación de nuestros archivos locales con los del servidor, si existiera alguna diferencia nos pediría realizar un get pull para realizar un match de nuestros archivos locales.

git fetch
```

```
Cuando un nuevo desarrollador se incorpora al equipo debe tener una copia del código y trabajarlo de forma local. Para descargar un repositorio completo basta con tomar la url y ejecutar el siguiente comando en alguna carpeta de su computadora.

git clone https://github.com/ElliotXLeo/AprendizajeGit.git
```

```
Cambiar tu URL remota de SSH a HTTPS con el comando git remote set-url.

git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```


