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



### GitHub \(o Bitbucket\)
- Git puede usarse localmente y sin conectarse a ningún otro equipo.
- No obstante el uso de un servidor remoto:
    - Facilita la compartición de código
    - Facilita el trabajo en equipo
    - Aumenta la seguridad de nuestro código.


### Uso de GitHub o Bitbucket
* Nos registramos en [Github](https://github.com/) o [Bitbucket](https://bitbucket.org)
* La comunicación entre un repositorio local y uno remoto puede ser mediante https o ssh.
* Por cuestiones prácticas consideramos mejor usar ssh. Veamos que configuración requiere.


#### Configuración de ssh
* Evitaremos introducir usuario/contraseña en nuestra consola
* Accedemos a nuestra cuenta
* Vamos a los settings del __USUARIO__ y asociamos una ssh-key
* Como creamos nuestra ssh-key:

```
ssh-keygen
```

* Copiaremos el contenido de  `~/.ssh/id\_rsa.pub`  a una nueva clave ssh en GitHub



# Uso de GIT: Iniciar el repositorio


## Para empezar.

- Podemos iniciar el repositorio en GitHub o Bitbucket
- Podemos iniciarlo localmente.
- Supongamos que hemos iniciado nuestro proyecto y tomamos la segunda opción.


## Objetivo
- Tomar una carpeta como nuestro repositorio.
- Puede ser la carpeta de ejercicicios de programación.
- Puede ser la carpeta de un proyecto concreto.


### ¿Qué hago localmente?
- Voy a git bash y me muevo a mi directorio
- Tecleo lo siguiente:
	- git init
	- echo "# Repositorio de ejemplo" >> README.md
	- git add README.md
	- git commit -m "Commit inicial"
	
### ¿Qué hago en GitHub/Bitbucket?

- Creo repositorio
- Sigo las instrucciones para subir mi repositorio local:


## Opción B. Iniciar el repositorio en GitHub/Bitbucket

- Al crear el repositorio se da la posibilidad de añadir un fichero README.md y crear un commit inicial.
- Por otra parte podemos partir de un repositorio nuestro o ajeno ya creado.
- En tal caso basta con hacer:

    ```
    git clone <url repo>           #habitual
    git clone <url repo> <carpeta> #permite definir destino
    ```


    