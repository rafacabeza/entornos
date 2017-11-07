# Control de versiones, documentación y optimización.



## SCV o Sistema de Control de versiones

Tomado del siguiente [Manual GIT](https://git-scm.com/book/es/v2) en [https://git-scm.com/book/es/v2](https://git-scm.com/book/es/v2):

_Un control de versiones es un sistema que registra los cambios realizados en un archivo o conjunto de archivos a lo largo del tiempo, 
de modo que puedas recuperar versiones específicas más adelante._


## SCV  centralizados

- El enfoque tradicional de los SCV es el de un sistema centralizado. 
- Es el caso de los muy utilizados CVS O Subversion. 
- Esto es fácil de administrar pero obliga a que el servidor siempre esté disponible.


## SCV  distribuidos

- Git, como Mercurial, Bazaar o Darcs, es un sistema distribuido. 
- Los clientes mantienen una copia completa de todo el repositorio.  
- Esto permite hacer cambios sin estar conectados. 
- En algún momento deben sincronizarse los clientes y el servidor o serviodres.


## Git
- Linux usaba BitKeeper para su desarrollo pero en 2005 dejó de ofrecer una licencia gratis para el proyecto GNU/Linux.
- Git se creó para sustituir a BitKeeper
- Linus Torvaldas, creador de Linux, desarrolló Git para dar soporte al desarrollo de este SO.


### Las características de git:

* Es distribuido
* Sencillo y rápido
* Permite grandes proyectos con mulititud de ramas
* Usa copias completas. Hace copia de los ficheros modificados y enlaces a los no modificados.
* Asegura la integridad. Realiza un hash SHA-1 a cada fichero. Si un fichero es alterado git lo detecta.


## Instalación
* Vamos a usar Ubuntu o alguna de sus variantes (Mint, Lubuntu, ...)
* Instalación de git:

  ```
  sudo apt-get update

  sudo apt-get install git
  ``` 
* En Windows, descargamos desde [aquí](https://git-scm.com/download/win) y ejecutamos.


## Configuración inicial

* Configuración necesaria para cada commit que haga:

  ```
  git config --global user.name "Your Name"

  git config --global user.email "youremail@domain.com"
  ```

* Opcionalmente el editor \(si no me gusta el que hay por defecto\):

  ```
  git config --global core.editor vi
  ```

## Niveles de configuración de git

Todo lo aquí contado puede verse con más detalle en el citado manual.

* Git tiene 3 niveles de configuración, cada nivel sobreescribe el anterior:

  * Para todos los usuarios: _/etc/gitconfig_

  * Para un usuario: _~/.gitconfig_ \(opción --global\)

  * Para un repositorio: _.git/config_

* Para ver los parámetros configurados:

```
git config --list
```

* Viene bien tener una [chuleta de comandos de Git](https://services.github.com/kit/downloads/github-git-cheat-sheet.pdf)

### Configuración de GitHub \(o Bitbucket\)

* Nos registramos en [Github](https://github.com/)

* Accedemos a nuestra cuenta

* Vamos a los settings y asociamos una ssh-key

  * Evitaremos introducir usuario/contraseña en cada _git push_

* Como creamos nuestra ssh-key:

```
ssh-keygen
```

* Copiaremos el contenido de _~/.ssh/id\_rsa.pub_ a una nueva clave ssh en GitHub



