# Indice

## Curso de Estadística Computacional con Python

### Objetivos del Curso

Objetivos

* Aprender cuándo utilizar Programación Dinámica y sus beneficios
* Entender la diferencia entre programas deterministas y estocásticos
* Aprender a utilizar Programación Estocástica
* Aprender a crear simulaciones computacionales válidas

### Introducción a la Programación Dinámica

En la década de los 50s Richard Bellman necesitaba financiamiento del gobierno para poder continuar con sus investigaciones, por lo que necesitaba un nombre rimbombante para que no fueran capaz de rechazar su solicitud, por lo que eligió programación dinámica. Las propias palabras de Bellman fueron:

"[El nombre] Programación Dinámica se escogió para esconder a patrocinadores gubernamentales el hecho que en realidad estaba haciendo Matemáticas. La frase Programación Dinámica es algo que ningún congresista puede oponerse." - Richard Bellman.

Ya sabiendo que Programación Dinámica no esta relacionado con su nombre, lo cierto es que si es una de las técnicas mas poderosas para poder optimizar cierto tipos de problemas.

Los problemas que puede optimizar son aquellos que tienen una subestructura óptima, esto significa que una solución óptima global se puede encontrar al combinar soluciones óptimas de subproblemas locales.

También nos podemos encontrar con los problemas empalmados, los cuales implican resolver el mismo problema en varias ocasiones para dar con una solución óptima.

Una técnica para obtener una alta velocidad en nuestro programa es la Memorización, el cual consiste en guardar cómputos previos y evitar realizarlos nuevamente. Normalmente se utiliza un diccionario, donde las consultas se pueden hacer en O(1), y para ello hacemos un cambio de tiempo por espacio.

**Programación Dinámica**

* Subestructura Óptima. Una solución global óptima se puede encontrar al combinar soluciones óptimas de subproblemas locales.
* Problemas empalmados. Una solución óptima que involucra resolver el mismo problema en varias ocasiones.

**Memoization**

* La Memorización es una técnica para guardar cómputos previos y evitar realizarlos nuevamente.
* Normalmente se utiliza un diccionario, donde las consultas se pueden hacer en O(1).
* Intercambia tiempo por espacio.

### Optimización de Fibonacci

![alt text](image.png)

### ¿Qué son los caminos aleatorios?

* Es un tipo de simulación que elige aleatoriamente una decisión dentro de un conjunto de decisiones válidas
* Se utiliza en muchos campos del conocimiento cuando los sistemas no son deterministas e incluyen elementos de aleatoriedad
