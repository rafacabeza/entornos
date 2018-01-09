# Diseño y realización de pruebas.



## Introducción

Su finalidad es:

- Verificar: el sofware hace lo que queremos que haga
- Validar: el software hace lo que el cliente espera7
- Todo antes de ponerlo en producción
- Son parte del ciclo de vida
- La tendencia es integrarlas en la fase de desarrollo


### Fases:
 - Planificación
 - Diseño y construcción de los casos de pruebas
 - Definición de los procedimientos
 - Ejecución de las pruebas
 - Registro de los resultados y análisis
 - Depuración de los errores
 - Informe de resultados


### Caso de prueba
Conjunto de entradas, condiciones de ejecución y resultados 
esperados para un objetivo particular o condición de prueba.
 - Hay que definir las condiciones (pre- y post-)
 - Hay que definir los valores de entrada
 - Hay que definir el comportamiento esperado
 - Analizar: pasa o no pasa la prueba



## Técnicas

- Caja Negra o funcionales: Analizar la funcionalidad sin conocer el codigo.
- Caja Blanca o estructurales: Analizar la estructura del codigo y ponerala a prueba.
![](img/cajaNegraBlanca.jpg)


### Pruebas de caja  blanca
Se basan en examinar minuciosamente los detalles procedimentales del código de la aplicación.
Mediante esta técnica se pueden obtener casos que:
 - Garanticen que se ejecutan al menos una vez todos los caminos independientes de cada módulo.
 - Ejecuten todas las sentencias al menos una vez.
 - Ejecuten todas las decisiones lógicas en su parte verdadera y en su parte falsa.
 - Ejecuten todos los bucles en sus límites.
 - Utilicen todas las estructuras de datos internas para asegurar su validez.


### Pruebas de caja negra

- Comprueban que el codigo hace lo esperado
- El resultado obtenido es el correspondiente a los datos aportados.
- No nos preocupamos de la estructura del software ni como funciona.
- Los casos de uso buscan demostrar que las salidas son las esperadas.


#### Errores obtenidos en pruebas de caja negra
 - Funcionalidades incorrectas/ausentes
 - Errores de interfaz
 - Errores de estructura de datos o acceso a BBDD
 - Errores de rendimiento
 - Errores de inicialización/finalización.



## Estrategias de Pruebas de Software
 - Pruebas de unidad: se centran en la unidad más pequeña de software, el módulo.
 - Pruebas de integración: se construye con los módulos una estructura de programa tal como dicta el diseño. 
 - Prueba de validación o aceptación: prueba del software en el entorno real de trabajo por el usuario final. Se validan los requisitos establecidos.
 - Prueba del sistema: verifica que cada elemento encaja de forma adecuada y se alcanza la funcionalidad y rendimiento total. 



## Pruebas de código


### Particiones equivalentes
- Dividimos los valores de entrada en particiones o clases equivalentes.
- Se debe probar el programa para un elemento de cada clase de equivalencia.
- Probado un valor, probados todos.


### Análisis de valores límites

- Se trata de probar los valores límite de las clases de equivalencia

### Pruebas aleatorias

- Se trata de obtener grandes baterias de pruebas de forma aleatoria
- Adecuado para entornos no interactivos