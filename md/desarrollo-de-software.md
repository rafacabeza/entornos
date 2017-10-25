# Software



## Definiciones:

* RAE: El conjunto de programas, instrucciones y reglas informáticas para ejecutar ciertas tareas en una computadora
* Estándar 729 IEEE: “El conjunto de los programas de cómputo, procedimientos, reglas, documentación y datos asociados que forman parte de las operaciones de un sistema de computación.
* Wikipedia: Se conoce como software al equipo lógico o soporte lógico de un sistema informático.


## Tipos:

* Sistema Operativo
* Software de desarrollo
* Aplicacioines informáticas.


## Sistema Operativo.

  * Software que permite usar el hardware de forma fácil y transparente.
  * Capa que se coloca entre el hardware y el resto de aplicaciones.


## Aplicaciones Informáticas.
  * Software que corre sobre el sistema operativo.
  * Software con una finalidad concreta.


## Software de desarrollo \(o CASE\).
  * Caso especial de aplicaciones.
  * Permite desarrollar nuevas aplicaciones.
  * Su estudio es parte fundamental de este módulo.


### Ejercicio

Haz tres listas de 5 elementos software que conocezcas de los tres tipos enumerados:

* Sistamas Operativos
* Aplicaciones informáticas
* Software de desarrollo.



# Distribución de software

De acuerdo al modo de distribución, podemos hablar de distintos tipos de sofware:


## Propietario o PRIVATIVO

* Controlado privadamente.
* No se puede acceder a su código fuente de forma libre.
* El código se encuentra en poder del desarrollador o compañía.
* No se permite su modificación, adaptación ni lectura por parte de terceros.


## Shareware

* Evaluación gratuita del producto.
* Límite de tiempo de evaluación.
* Restricciones en las capacidades finales.
* Requiere un pago para uso completo.
* También “shareware de precio cero”
* WinRAR, PC File, Paint Shop Pro, PC-Tools,Virus Scan…


## Adware

* Software de publicidad.
* Incluidos en programas Shareware.
* Muchas veces se puede evitar su descarga si estamos atentos.
* Comprando la licencia del Shareware también eliminamos la publicidad.


## Freeware

* Se distribuye sin coste.
* No confundir con código libre:
* Mantiene el Copyright.
* NO se puede modificar.
* NO se puede utilizar libremente \(modificar ni vender\).
* Ofrece funcionalidad completa de manera gratuita.
* Suele incluir licencia comercial


## Software Libre

* Puede ser:
  * Utilizado
  * Estudiado
  * Distribuido
  * Mejorado
* No tiene por qué ser gratuito.
* Puede ser distribuido comercialmente.
* Muy común utilizar licencia GNU GPL.



## Software de Uso Específico

* Se desarrolla para resolver una necesidad determinada en una organización o persona.
* Requiere expertos informáticos para
  * Desarrollo
  * Adaptación
* Ej: Videoclub, Generación de Horarios, Faltas de asistencia, Banca.
* Es el software que más trabajo supone para las empresas de desarrollo.



## Fases del desarrollo del software

Aunque esta cuestión será revisada y analizada con más detenimiento al final del curso,  vamos a enumerar las fases de un desarrollo software.

A este conjunto de tareas nos referimos como ciclo de vida del software.


* Análisis
* Diseño
* Codificación
* Pruebas
* Documentación
* Explotación
* Mantenimiento



# Herramientas CASE

* CASE. Computer Aided Software Engineering.
* Aplicaciones cuya finalidad está relacionada con el desarrollo del software.
* Son aplicaciones destinadas a aumentar la productividad en el desarrollo de software reduciendo costes en términos de tiempo y de dinero


## Herramientas vs entornos


### Herramientas

* Hablamos de herramientas para referirnos a aplicaciones que dan soporte a una tarea concreta dentro del ciclo de vida.
* Su uso se circunscribe a una sóla de las fases del ciclo de vida.


* Algunas de ellas:
  * Herramientas de modelado, para reflejar el análisis del negocio. Los modelos habituales son E/R y UML 
  * Herramientas de desarrollo: editores de código, compiladores, depuradores, enlazadores, ...
  * Gestión de proyectos: para planificar los proyectos, asignar tareas, los tiempos, etc.
  * Herramientas de verificación y validación, usadas para analizar la corrección del código y su rendimiento.
* Podemos referirnos a ellas como Upper-CASE y Lower-CASE Tools. Las Upper o altas dan soporte a las fases de análisis y diseño. Las Lower-CASE dan soporte a las fases de desarrollo y siguientes. Esta clasificación no siempre es adecuada.


### Entornos

* Las herramientas CASE pueden agruparse en un único software. Este tipo de software que ayuda en multitud de tareas del desarrollo de software puede ser referido como _**workbench**_** **o más habitualmente como entorno, o _**environment**_.
* Las siglas IDE \(Integrated Development Environment\) son usadas habitualmente para estos entornos.
* Un IDE es una aplicación informática que proporciona servicios integrales para facilitarle al desarrollador o programador el desarrollo de software.



## Concepto de Programa
- 	Conjunto de instrucciones escritas en un lenguaje de programación que aplicadas sobre un conjunto de datos resuelven un problema o parte del mismo.
- 	Es necesario traducirlo a lenguaje máquina. Esto lo hace el compilador. 
- 	Después, se carga en memoria principal para que el procesador ejecute una a una todas las instrucciones.



## Concepto de Lenguaje
- 	Conjunto de caracteres, reglas para la combinación de esos caracteres y reglas que definen sus efectos cuando los ejecuta un ordenador.
- 	Pueden usarse para crear programas que controlen el comportamiento físico y lógico de una máquina, para expresar algoritmos con precisión, o como modo de comunicación humana.


### Clasificación y características


#### Según su nivel de abstracción
   - Lenguajes de bajo nivel: código máquina o ensamblador
   - Lenguajes de alto nivel: lenguaje próximo al hombre (p. ej. Java)
   - Lenguajes de nivel medio: caractarísticas de ambos (p. ej. C)


##### 	Lenguajes de bajo nivel
   - 	Cerca del funcionamiento del ordenador
   - 	El más bajo es el lenguaje máquina
        - Instrucciones formadas por 0s y 1s.
   - 	Le sigue el lenguaje ensamblador. 
        -	Específico para cada procesador.
        -	Necesita ser traducido a lenguaje máquina.
        -	Las instrucciones trabajan directamente con registros de memoria física de la máquina.


##### 	Lenguajes de medio nivel
   - 	Características que los acercan a lenguajes de bajo nivel pero también características de los lenguajes de alto nivel.
   - 	Se suelen utilizar para creación de SO, drivers, controladores, ...
   -    Cerca del hardware para lograr más eficiencia.
   - 	Ejemplo: C


##### 	Lenguajes de alto nivel
   - 	Fáciles de aprender, formados por palabras del lenguaje natural.
   - 	Necesitan de un intérprete o un compilador para ser ejecutados, que traduzca las instrucciones escritas en lenguaje máquina.
   - 	Son independientes de la máquina.
   - 	Ejemplos: Java, PHP, Visual .Net, COBOL, Python, C++, etc.


### Según la forma de ejecución
   - 	Lenguajes compilados. Hay conversión previa a código máquina.
   - 	Lenguajes interpretados. A la vez se convierte y se ejecuta.


####	Lenguajes compilados
   - 	El compilador traduce de un determinado lenguaje a un programa equivalente. 
   - 	El compilador devolverá errores si el programa en el lenguaje fuente no está bien escrito. 
   - 	El programa generado es más rápido que uno interpretado.


####	Lenguajes interpretados
   - 	Los intérpretes, en vez de producir un programa destino como resultado, nos da la apariencia de ejecutar directamente las operaciones especificadas en el programa fuente con las entradas proporcionadas por el usuario. 
   - 	Cada vez que se ejecuta una instrucción se debe interpretar y traducir a lenguaje máquina.
   - 	El intérprete elimina la necesidad de realizar una compilación después de cada modificación.
   - 	Ej: PHP, Java Script, Python, Ruby, etc.


   
### Según el paradigma de programación
   - Lenguajes imperativos
   - Lenguajes declarativos:
      - Lenguajes funcionales
      - Lenguajes lógicos
   - 	Lenguajes estructurados
   - 	Lenguajes orientados a objetos


#### ¿Qué es el paradigma?
- 	El paradigma es un enfoque particular para la construcción del software.
- 	Define un conjunto de reglas, patrones y estilos de programación.
- 	Dependiendo del problema a resolver, un paradigma resultará más apropiado que otro.


####  	Lenguajes imperativos
   - 	Indican al ordenador CÓMO realizar una tarea.
   - 	La sentencia principal es la asignación.
   - 	Instrucciones simples.
   - 	Los primeros fueron los lenguajes máquina y ensambladores.


####  Lenguajes Declarativos

- Declaran QUÉ hacer
- Se definen las condiciones de cálculo.
- No se codifica orden por orden.


####  	Lenguajes funcionales
   - 	Basado en el concepto matemático de función.
   - 	No existe la operación de asignación. 
   - 	Las variables almacenan definiciones o referencias a expresiones.
   - 	La operación fundamental es la aplicación de una función a una serie de argumentos.
   - 	Poco utilizados.


####  	Lenguajes lógicos
   - 	En ellos un cálculo es el proceso de encontrar qué elementos de un dominio cumplen o no alguna relación definida sobre dicho dominio.
   - 	Se pueden ver como bases de datos formadas por listas de reglas. 
   - 	La ejecución consistirá en realizar preguntas
   - 	Ej: Prolog, Sistemas expertos, demostración de teoremas, etc.


#### 	Lenguajes estructurados
   - 	Utilizan estructura secuencial, condicional y repetitiva. 
   - 	Pueden ser leídos secuencialmente desde el comienzo hasta el final sin perderse.
   - 	Problema: Si es demasiado grande, resulta difícil su lectura y manejo.
   - 	Actualmente con programación estructurada nos referimos a la división de un programa en módulos más manejables, con sus entradas y salidas.


#### 	Lenguajes Orientados a Objetos
   - 	Los programas están compuestos por un conjunto de objetos.
   - 	Un objeto consta de una estructura de datos (atributos) y de una colección de métodos u operaciones que manipulan esos atributos. Las operaciones definen el comportamiento de los objetos y cambian valores de sus atributos.
   - 	Las clases son plantillas para la creación de objetos. Al crear un objeto hay que indicar de qué clase es.



### 	Código fuente:
   - 	Es el escrito por los programadores.
   - 	Se utiliza un lenguaje de programación de alto nivel.
   - 	Tradicionalmente se parte de los diagramas de flujo o pseudocódigos diseñados en la etapa de diseño.
   - 	No es directamente ejecutable por el ordenador.


####  	Código objeto
   - 	Es el código resultante de compilar el código fuente.
   - 	No es directamente ejecutable por el ordenador ni entendible por el ser humano.
   - 	Es un código o interpretación intermedia de bajo nivel.


####  	Código ejecutable
   - 	Es el resultado de enlazar el código objeto con una serie de rutinas y librerías.
   - 	Es directamente ejecutable por la máquina.




   Compilación
- 	Se lleva a cabo mediante dos programas: el compilador y el enlazador.
- 	El compilador puede devolver errores, que habrá que subsanar y harán que no se genere el código objeto.
- 	El enlazador inserta en el código objeto las funciones de librería necesarias para producir el programa ejecutable. 
Compilación
Compilación
- 	Se compone internamente de varias etapas o fases (1/2):
   - 	Análisis léxico: Lee todo y lo convierte a tokens.
   - 	Análisis sintáctico: Lee los tokens y los analiza.
   - 	Análisis semántico: Comprueba las declaraciones, los tipos de las expresiones, si las operaciones se pueden realizar sobre esos tipos, si los tamaños son adecuados…
Compilación
- 	Se compone internamente de varias etapas o fases (2/2):
   - 	Generación de código intermedio: similar al código máquina para facilitar la traducción al código objeto.
   - 	Optimización de código: para que sea más fácil y rápido de interpretar por la máquina.
   - 	Generación de código: genera el código objeto de nuestro programa.

   
   
   
   
   
   

La Máquina Virtual de Java
- 	Una máquina virtual es una aplicación software de una máquina que ejecuta programas como si fuese la máquina real.
- 	Los programas compilados en lenguaje Java se pueden ejecutar en cualquier plataforma porque el código generado por el compilador no lo ejecuta el procesador del ordenador sino la JVM.
La Máquina Virtual de Java
- 	Funcionamiento:

La Máquina Virtual de Java
- 	Tareas principales de la JVM:
   - 	Reservar espacio en memoria para los objetos creados y liberr la memoria no utilizada.
   - 	Comunicarse con el sistema huésped (ej. controlar el acceso a hardware)
   - 	Vigilar el cumplimiento de las normas de seguridad de las aplicaciones Java
UD 1. Desarrollo de Software
- 	Introducción
- 	Tipos de software
- 	Ciclo de vida del software (breve)
- 	Fases del desarrollo (breve)
- 	¿Qué es un programa?
- 	Lenguajes de programación
- 	Tipos de código y compilación
- 	La máquina virtual de Java
- 	Ejemplos DFD y Pseudocódigo

DFD y Pseudocódigo
- 	Símbolos de Diagrama de Flujo de Datos:
DFD y Pseudocódigo
- 	Símbolos de Pseudocódigo:
