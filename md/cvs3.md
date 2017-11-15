## Uso de git: guardar cambios
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
la rama master.
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