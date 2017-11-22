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
* La mayoría de cambios se hacen localmente.


### Esquema de almacenamiento

- Cada instantánea se identifica por un _hash_ SHA1
- Cada instantánea o _commit_ añade los ficheros modificados. Y guarda enlaces al resto.

![](img/gitHistory.png)
