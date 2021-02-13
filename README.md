# AprendizajeGit
Aprendizaje de Git desde 0.
En este repositorio muestro como voy aprendiendo poco a poco los comandos de git bash.

Espero aprender mucho.

![alt text](https://miro.medium.com/max/352/1*qR6xp69TZSS9Dv_ZBxTw1w.jpeg)

## Comandos empleados en el aprendizaje
```
Brinda ayuda sobre los comandos

git <comandos>* help
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
Lista el estado de los archivos 

git status
```

```
Agrega todos los archivos pendientes de cambios

git add --all
```

```
Captura estado del código y lo almacena en el repositorio local. Posterior a git add *

git commit -m "<descripción>"
```

```
Deshace la captura del estado del código

git reset
```

```
Abre un editor de texto con el último commit y vuelve a realizar el commit al salir de este.
También es útil para adicionar una modificación.

git commit --amend
```

```
Muestra los commit realizados hasta el momento

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
Cambia a un commit en específico por su código.

git checkout <código>
```

```
Cambiamos a un commit en específico por su código con el objetivo de volver a empezar desde ese punto.

git reset --hard <código>
```

```
Crea una nueva rama

git branch nombreRama
```

```
Nos muestra en que rama estamos y lista las demás

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
Permite juntar dos ramas, desde la rama principal invocando a la rama que se quiera unir a esta.

git merge nombreRama
```

```
Permite juntar dos ramas, pero mantiene la existencia de cada una de forma que se puede ver un gráfico de ramas.

git merge --no-ff develop
```

```
Crea un tag

git tag nombreTag -m "Versión alpha"
```

```
Lista tags

git tag
```

```
Borra un tag en específico

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
#### Para subir nuestro proyecto debemos crear un repositorio remoto. Al crearlo nos mostrará una serie de comandos para subir el proyecto. Te pedirá el usuario y contraseña de tu cuenta de git si aún no lo registras.

```
Vincular repositorio remoto con repositorio local 

git remote add origin https://github.com/ElliotXLeo/AprendizajeGit.git
```

```
Subir archivos del repositorio local al remoto

git push -u origin master
```

```
Nos muestra en que repositorio estamos enlazados remotamente.

git remote -v
```

```
Sube todos los cambios locales al servidor remoto de Git.

git push
```

```
Sube todos los tags al repositorio remoto,.

git push --tags
```

```
Hace push a un repositorio remoto en otras ramas que no sea la de por defecto

git push origin <nombreRama>
```

```
Descarga el contenido desde un repositorio remoto y actualiza el repositorio local en la rama por defecto

git pull
```

```
Descarga el contenido desde un repositorio remoto y actualiza el repositorio local en una rama específica

git pull origin <rama>
```

```
Compara nuestros archivos locales con los del servidor, si existiera alguna diferencia nos pediría realizar un get pull para realizar un match de nuestros archivos locales.

git fetch
```

```
Clona un repositorio remoto en la rama por defecto

git clone https://github.com/ElliotXLeo/AprendizajeGit.git
```

```
Clona un repositorio remoto en una reama específica

git clone --branch <rama> <https://github.com/ElliotXLeo/AprendizajeGit.git>
```
