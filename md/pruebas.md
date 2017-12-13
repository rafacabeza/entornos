# Diseño y realización de pruebas.



## Introducción

Su finalidad es:

- Verificar: el sofware hace lo que queremos que haga
- Validar: el software hace lo que el cliente espera


### Fases:
 - Planificación
 - Diseño y construcción de los casos de pruebas
 - Ejecución
 - Registro de los resultados y análisis
 - Deuración
 - Informe de errores


## Técnicas

- Caja Negra o funcionales: Analizar la funcionalidad sin conocer el codigo.
- Caja Blanca o estructurales: Analizar la estructura del codigo y ponerala a prueba.


## Pruebas de caja negra

- Comprueban que el codigo hace lo esperado
- El resultado obtenido es el correspondiente a los datos aportados.
- No nos preocupamos de la estructura del sofware


### Particiones equivalentes
- Dividimos los valores de entrada en particiones o clases equivalentes.
- Se debe probar el programa para un elemento de cada clase de equivalencia.
- Probado un valor, probados todos.


### Análisis de valores límites

- Se trata de probar los valores límite de las clases de equivalencia

### Pruebas aleatorias

- Se trata de obtener grandes baterias de pruebas de forma aleatoria
- Adecuado para entornos no interactivos