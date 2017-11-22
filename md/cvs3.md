## Uso de git: guardar cambios
Todas estas operaciones son locales:
- No es necesario salir a la red
- Velocidad muy alta de las operaciones
- Lee de tu base de datos local
- Calcula diferencias entre ficheros en local
- No limita el trabajo sin conexión


### Ver el estado
- Consultar el estado del repositorio: `git status`
- Nos dirá qué ficheros hay nuevos o modificados
- La rama que estamos, por defecto master
- Si estamos por detrás/delante del _origin_, el repositorio remoto

![git status](img/git1.png "Logo Title Text 1")


### Preparar y comprometer cambios:

- Con `git add ...` pasamos los ficheros modificados/nuevos a preparados.
- Tras hacer esto se guarda temporalmente los cambios realizados.
- Con `git commit -m "...." comprometemos los cambios.

```
git add .
git commit -m "comentario explicativo"
```

![git status](img/git2.png "Ejemplo de commit")


#### Ejemplos de  `git add`

```
git add <nombre fichero>    #un sólo fichero
git add img/logo.jpg
git add <nombre directorio> #todo lo de un directorio
git add .                   #caso particular, todo, todo...
git add public/js
```


#### Recorrido completo:


![git status](img/git03.png)
![git status](img/git04.png)


![git status](img/git05.png)
![git status](img/git06.png)


#### Marcha atrás de un fichero modificado

- Hemos modificado un fichero y queremos recuperar la anterior versión:

![git status](img/git03.png)
```
git checkout <nombrefichero>
git checkout casa.md
git checkout <nombre directorio>
git checkout .
```


#### Marcha atrás de un fichero preparado

- Queremos sacar del estado preparado después de `git add`:

![git status](img/git04.png)
```
git reset HEAD <nombrefichero>
git reset HEAD casa.md
git reset HEAD <nombre directorio>
git reset HEAD .
```



### Guardar en remoto.
- En local por defecto trabajamos en la rama master.
- Si hay un remoto, además se guarda oculta la rama origin/master.
- Sean los equipos A y B, y mismo repositorio:

![](img/gitremote01.png)


#### Commit + push, equipo A

![](img/gitremote02.png)
![](img/gitremote03.png)


#### Git push
- Push es el comando usado para subir código a _origin_, es decir
el repositorio remoto.
- Origin es el nombre usado por defecto para la copia remota.
- Ejemplos de uso

```
git push                        # sube rama "preferida"

# comando usado en la subida inicial tras git init. Lo explicaremos
git push -u origin master       
```


#### Fetch + pull, equipo B
- Se recomienda hacer git status entre ambos.
- En realidad pull es la suma de dos comandos: fetch + merge

![](img/gitremote04.png)
![](img/gitremote05.png)


### ¿Cómo usar dos equipos: aula y casa?

- Al empezar a trabajar, ejecutar
```
git fetch
git status
git pull
```
- Al acabar la sesión de trabajo
```
git commit 
git status
git push
```


### Fork & Pull Request
#### Fork
- Clon de un repositorio ajeno en nuestro espacio
- Es una funcionalidad de GitHub/Bitbucket
- P.ej. el repositorio repo1702
- El clon es de mi propiedad y lo puedo clonar 
y editar
#### Pull Request
- Es una solicitud de que el dueño original 
incorpore mis cambios.
- Se hace en la interfaz web
- El dueño original lo acepta o no...


### Commit --amend
- Consiste en rectificar el commit anterior
- Los cambios añadidos sobreescriben el último
commit
- OJO! Puede ser peligroso.



## Ramas (branch)
- Por defecto trabajamos en la rama `master`
- Las ramas se usan fundamentalmente para separar tareas sin
modificar la rama `master`
- Una vez terminada la tarea se funde (merge) la rama de tarea 
con la rama master.
- Esto permite cambiar de rama/tarea y dejarla incompleta sin
dejar el proyecto en versiones incompletas o inestables.


### Comandos con ramas
```
git branch              // lista de ramas
git branch  <rama>      // crear rama
git checkout <rama>     // cambiar de rama
git checkout -b <rama>  // crear y cambiar rama 2 en 1
git branch -d <rama>    // borrar rama
```
### Fundir ramas
```
git checkout master     // nos ponemos en rama master
git merge <rama>        //fundimos con la rama deseada
```


### Revisemos el uso de push 
- Push sube código a un repositorio remoto
- Origin es el alias usado pra el repositorio remoto
- Podríamos usar más de un remoto
- Master es el nombre de la rama por defecto
```
git push                        # sube rama "preferida"
git push <repo remoto> <rama>   # sube una rama concreta
git push origin dev             # Ej. sube rama dev
git push -u <repo remoto> <rama># sube y predetermina rama
git push -u origin master       # Ej. sube y pred. master
```


### Ramas remotas
- Si queremos compartir una rama de trabajo
- Subir una rama:
```
git push origin <rama>
```
- Bajar la rama tiene dos partes:
```
git fetch  #crea la rama oculta origin/<rama>
```
- Las siguientes ordenes son idénticas.
- Ambas crear la rama local <rama> asociada a origin/<rama> 
- La primera nos permite alterar el nombre <rama>.
```
git checkout -b <rama> origin/<rama>
git checkout --track origin/<rama>
```



## Revisando código
- Los comandos básicos son log y diff
- `git log` nos muestra información histórica
- `git diff` compara el contenido de los ficheros


### log
- Log soporta una gran cantidad de parámetros:
- Veámoslo con ejemplos:
```
git log             #uso base
git log -<n>        #log de los últimos n commits
git log 
```



## GitIgnorando cosas: .gitignore

- Podemos decir a git que no tenga en consideración algunos ficheros/directorios
- Para hacerlo debemos crear un fichero `.gitignore` en el directorio raiz
- Para ver algunos ejemplos puedes visitar https://www.atlassian.com/git/tutorials/gitignore