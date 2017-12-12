# Documentacion



## ¿Qué y cuándo documentar?

- Análisis: especificaciones
- Diseño: descripción de la arquitectura.
- Implementación: código fuente.
- Pruebas: plan de pruebas.
- Documentacion de usuario.


## ¿Por qué documentar el código?

- Un programa con éxito:
    - Necesitará arreglar errores
    - Evolucionará
- La documentación ayudará a entender el código
    - Al propio autor del código
    - A cualquier programador nuevo en el proyecto


### Citas

    > If your program isn't worth documenting, it probably isn't worth running
    
    J. Nagler. 1995
    Coding Style and Good Computing Practices 

    > Do not document bad code - rewrite it
    
    R. Caron. 2000
    Coding Techniques and Programming Practices 

    > Write the documentation before you write the code.
    
    S.W. Ambler. 2000.
    Writing Robust Java Code 


### Comentarios

- Código autodocumentado
- De una línea: `// comentario de una línea`
- Multilínea `/* comentario multilínea*`
- Comentarios de JavaDoc `/** comentario multilínea JavaDoc *`


### Comentarios JavaDoc

- Primera parte descriptiva. Permite HTML
- Segunda parte tags JavaDoc:
    - @etiqueta descripción
    - El juego de etiquetas está normalizado
    - @author, @version, @see, @param, @return, @throws, @deprecated, @since


### Documentar clases e interfaces
 
------------------------------------------------------
| Etiqueta   |   Descripción                         |  Obligatoria |
------------------------------------------------------
| @author   |   nombre del autor                     |  Si |
------------------------------------------------------
| @version	|   identificación de la versión y fecha |  Si |
------------------------------------------------------
| @see      |   referencia a otras clases y métodos  |  - |
------------------------------------------------------

    