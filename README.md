# AprendizajeGit
Linea de aprendizaje de Git desde 0.
En este repositorio muestro como voy aprendiendo poco a poco a usar git bash desde 0, espero aprender muchas funcionalidades.

![alt text](https://miro.medium.com/max/352/1*qR6xp69TZSS9Dv_ZBxTw1w.jpeg)

## Comandos empleados en el aprendizaje
```
Brinda ayuda sobre los comandos

git [comandos] help
```
### Repositorio local
```
Configura el email y usuario, solo se hace una vez cuando se instala git

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
Captura estado del código y lo almacena en el repositorio local

git commit -m "primer commit"
```

```
Muestra en una línea de los commit realizados

git log --oneline
```

```
Viajamos a un commit en específico por su código y restauramos los archivos ejemplo: f52f3da

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
Nos movemos de al rama actual a una en específica

git checkout nombreRama
```

```
Eliminar una rama

git branch -d nombreRama
```

```
Crear un tag

git tag nombreTag -m "versión alpha"
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

git tag -a nombreTag f52f3da -m "version alpha"
```

```
Mostrar información del tag

git show nombreTag
```

### Repositorio remoto
#### Para subir nuestro proyecto debemos crear un nuevo repositorio, al momento de la creación nos mostrará una serie de comandos para subir el proyecto.

```
Vincular repositorio remoto con repositorio de origen local y subir archivos del repositorio origen local de la rama master

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
Cuando realizamos cambios directamente en GitHub, pero no de forma local, es esencial realizar un pull, donde descargaremos los cambios realizados para seguir trabajando normalmente. Es importante estar enlazados remotamente.

git pull
```

```
Este comando hace la comparación de nuestros archivos locales con los del servidor, si existiera alguna diferencia nos pediría realizar un get pull para realizar un match de nuestros archivos locales.

git fetch
```

```
Cuando un nuevo desarrollador se incorpora al equipo debe tener una copia del código y trabajarlo de forma loca. Para descargar un repositorio completo basta con tomar la url y ejecutar el siguiente comando en alguna carpeta de su computadora.

git clone https://github.com/ElliotXLeo/AprendizajeGit.git
```

```
Cuando se trabaja en diferentes ramas y lo que busca es juntar dos de ellas para que tengan el mismo código. Se emplea el siguiente comando desde la rama principal invocando a la rama que se quiera unir a esta.

git merge nombreRama
```

```
Cambiar tu URL remota de SSH a HTTPS con el comando git remote set-url.

git remote set-url origin https://github.com/USERNAME/REPOSITORY.git
```


