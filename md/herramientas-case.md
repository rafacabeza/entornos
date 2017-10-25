# Entornos de desarrollo



## Funciones de un Entorno de Desarrollo

Entorno de Desarrollo en inglés, Integrated Development Environment (IDE).
- Editar
- Compilar 
- Interpretar 
- Depurar
- Otras ...


### Componentes de un IDE
- Editor de texto 
- Compilador. Convierte código fuente a código máquina.
- Intérprete. Convierte el código fuente y lo ejecuta al vuelo. Sin guardar.
- Depurador (Debugger). Permite ejecutar paso a paso un programa e inspeccionar 
el estado del programa.
- Constructor de interfaz gráfica. Permite crear interfaces gráficas mediante un editor 
[WYSIWYG](https://es.wikipedia.org/wiki/WYSIWYG).
- Control de versiones. Para poder modificar el código
- Soporte para más de un lenguaje


#### Editor de texto
- Colorea variables, constantes, palabras reservadas, ...
- Marcar inicio/fin de paréntesis y corchetes
- Oculta/recoge bloques de código y funciones
- Marca errores


#### Compilador
- Traduce código fuente a código máquina

#### Intérprete
- Realiza la traducción al ejecutar
- No guarda resultado
- Más lento pero flexible para el programador
- El entorno de ejecución lo fija el IDE (VM)


#### Depurador o debugger
- Se usa para limpiar y depurar el código fuente
- Permite ejecutar paso a paso y examinar cómo se comporta el programa.
- Permite ver el contenido de las variables del programa o los registros del procesador en cada momento
- Permite parar el programa donde nos interes



## Instalación de un entorno de desarrollo 


### Instalación de Eclipse

- Instalación de Eclipse
- scargar de www.eclipse.org
- Versión Neon 3
- Descomprimir
- Ejecutar
- Seleccionar el Workspace: almacenes de proyectos de eclipse
- Nota: las versiones posteriores vienen con instalador típico


#### Importación de un proyecto

Forma 1:
- Menú File / Import
- General / Existing Projects into Workspace
- Seleccionar la carpeta de trabajo y marcar el proyecto.
Finish
Forma 2:
- Menú File / Open Projects from File System
- Import Source (Buscar directorio)
- Finish


#### Ventana principal de trabajo Eclipse
- Package Explorer: zona de proyectos, para navegar por el workspace.
- Zona de edición: escribir el código de los programas. Textos resaltados para identificar la sintaxis y palabras reservadas. Errores subrayados en rojo y se ofrecen soluciones. Propuestas de plantilla para simplificar la escritura
- Outline: esquema de la clase en edición. Métodos y atributos.
- Consola Java: resultado de la ejecución de los programas, salida por consola, errores ejecución


#### Window y Perspectivas
- La ventana principal es un mosaico de ventanitas o  **views**.
- La visualización de la ventana principal se puede cambiar desde el menú window.
- Se pueden activar otras vistas en Window / Show View.
- Las perspectivas:
    - Son un montaje de vistas determinado.
    - Existen perspectivas predefinidas.



### Instalación de plugins 
- Plugin: programa o aplicación que añade funcionalidades específicas a otro programa, en forma de complementos o extensiones. 
- Muy habituales en navegadores, reproductores de música y herramientas de desarrollo.
- No son parches ni actualizaciones.


#### Creación de nuevo proyecto con GUI
- File / New / Java Project
- Escribir nombre de proyecto
- Finish
- Sobre el proyecto, botón derecho New / Other / WindowBuilder / Swing Designer / Application Window
- Escribir nombre de la ventana
- Finish


#### Creación de nuevo proyecto con GUI
- La nueva clase con el nombre de la ventana se puede editar en modo fuente (source) o en modo diseño (design).
- En el modo diseño se distinguen bloques:
    - Structure: Componentes agregados jerárquicamente.
    - Properties: Propiedades del elemento seleccionado.
    - Palette: Elementos que se pueden añadir a la ventana.
    - Ventana o formulario: Donde se van añadiendo los elementos.

    
#### Creación de nuevo proyecto con GUI
- Para añadir componentes a la ventana primero hay que añadir un contenedor donde añadir elementos: Layouts.- 
- Cambia las propiedades: 
    - Nombre del control: Variable
    - Cambiar el aspecto: background, font, foreground, text, horizontalAlignment, verticalAlignment, etc.
    - Añadir funciones a los botones: doble click sobre el botón de la ventana y se visualiza actionPerformed. Las acciones se añadirán en este módulo.
    - Utiliza Absolute Layout para introducir los controles.
    - Utiliza JLabel, JTextField, JButton y JPanel (caja que encierra a los controles) para crear la ventana de la siguiente página.


#### Creación de nuevo proyecto con GUI
![imagen](img/ed1b.png "")


#### Creación de nuevo proyecto con GUI
- Añadimos ahora acción al botón de limpiar datos:
- Hacemos doble click sobre el botón y se visualiza el código actionPerformed.
- Para visualizar un mensaje cuando se pulsa el botón, por ejemplo, habrá que escribir el código en ese método. 
- Probamos lo siguiente:


#### Creación de nuevo proyecto con GUI
![imagen](img/ed1a.png "")

