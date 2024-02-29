# Indice

## Curso de Introducción al Pensamiento Computacional con Python

### Introducción al pensamiento computacional

Objetivos

* Aprender a resolver problemas de manera computacional
* Entender los puntos en común entre todos los lenguajes de programación
* Desarrollar las bases para una carrera en Computer Science

### Introducción al cómputo

**Resumen Introducción al Cómputo**

* **"Primera computadora"** creada por los griegos, calcula la posición del sol, luna y algunas constelaciones.

* En 1801, Telar de Jacquar, separa el resultado de la informacion que contiene las instrucciones.

* Siglo XIX, Motor analítico de Babbage, haciendo uso del avances en mecánica (engranajes) de su época logra separar instrucciones de calculo y realizar varios cálculos a la vez.

* Finales siglo XIX, ENIAC (Eectronic Numerical Integrator and Computer) usaba sistema decimal. creada por Alan Turing y Alonso. Esta época exigía exactitud en los cálculos que hacían que compañías dependieran de esta(Compañías Ferroviarias por ejemplo). Turing y Alonso, Descubrieron que matemáticamente todos los algoritmos podíamos reducirlos a una secuencia de soluciones matemáticas.

* En 1945, Arquitectura de Von Neumann, EDVAC (Electronic Discrete Variable Automatic Computer) usaba sistema binario. Su aporte fue el descubrimiento que dentro de los componentes electrónicos se puede usar una serie de hadward para realizar el computo y almacenar datos dentro de memoria.

* En 1950, Microchip, ejemplo Apple 1

* En siglo XX, Arquitectura de Feymann, aporta las bases matemáticas de computo cuántico.

![alt text](image.png)

Cómputo y computadoras

* Las computadoras hacen dos cosas: hacen cálculos y recuerdan el resultado de dichos cálculos.
* Por la mayoría de la historia humana, estábamos limitados por la velocidad del cerebro y la mano.
* Aún con las computadoras modernas existen problemas que no podemos resolver.

### Introducción a los lenguajes de programación

¿Qué es un lenguaje de programación? Es un lenguaje formal que, mediante una serie de instrucciones, le permite a un programador escribir un conjunto de órdenes, acciones consecutivas, datos y algoritmos para, de esa forma, crear programas que controlen el comportamiento físico y lógico de una máquina.

¿Qué tipos de lenguaje de programación existen? El lenguaje de programación es la base para construir todas las aplicaciones digitales que se utilizan en el día a día y se clasifican en dos tipos principales: lenguaje de bajo nivel y de alto nivel.

Lenguaje de programación de bajo nivel Son lenguajes totalmente orientados a la máquina.

Este lenguaje sirve de interfaz y crea un vínculo inseparable entre el hardware y el software.

Además, ejerce un control directo sobre el equipo y su estructura física. Para aplicarlo adecuadamente es necesario que el programador conozca sólidamente el hardware. Éste se subdivide en dos tipos:

Lenguaje máquina Es el más primitivo de los lenguajes y es una colección de dígitos binarios o bits (0 y 1) que la computadora lee e interpreta y son los únicos idiomas que las computadoras entienden.

Ejemplo: 10110000 01100001

No entendemos muy bien lo que dice ¿verdad? Por eso, el lenguaje ensamblador nos permite entender mejor a qué se refiere éste código.

Lenguaje ensamblador El lenguaje ensamblador es el primer intento de sustitución del lenguaje de máquina por uno más cercano al utilizado por los humanos.

Un programa escrito en éste lenguaje es almacenado como texto (tal como programas de alto nivel) y consiste en una serie de instrucciones que corresponden al flujo de órdenes ejecutables por un microprocesador.

Sin embargo, dichas máquinas no comprenden el lenguaje emsamblador, por lo que se debe convertir a lenguaje máquina mediante un programa llamado Ensamblador.

Este genera códigos compactos, rápidos y eficientes creados por el programador que tiene el control total de la máquina.

Ejemplo: MOV AL, 61h (asigna el valor hexadecimal 61 al registro “AL”)

Lenguaje de programación de alto nivel Tienen como objetivo facilitar el trabajo del programador, ya que utilizan unas instrucciones más fáciles de entender.

Además, el lenguaje de alto nivel permite escribir códigos mediante idiomas que conocemos (español, inglés, etc.) y luego, para ser ejecutados, se traduce al lenguaje de máquina mediante traductores o compiladores.

++Traductor++ Traducen programas escritos en un lenguaje de programación al lenguaje máquina de la computadora y a medida que va siendo traducida, se ejecuta.

++Compilador++ Permite traducir todo un programa de una sola vez, haciendo una ejecución más rápida y puede almacenarse para usarse luego sin volver a hacer la traducción.

**Programación**

* Turing completeness

* Los lenguajes de programación modernos dan primitivos que son más convenientes que los primitivos de Turing.

**Lenguajes**

**Sintaxis** Define la secuencia de símbolos que está bienformada.

**Semántica estática** Define qué enunciados con sintaxis correcta tienen significado

**Semántica** Define el significado. En los lenguajes de programación sólo hay un significado.

### Preparación de tu computadora

Antes de comenzar este curso asegúrate de preparar tu entorno de trabajo para poder hacer todos los ejercicios. A continuación te compartiré los pasos que debes seguir para configurar tu computadora.

Si estás usando Windows asegúrate de instalar lo siguiente en tu computadora:

Python 3.7 (o superior)

1. Para obtener el instalador dirígete a <https://www.python.org/downloads/>

![alt text](image-1.png)

2. Descarga el instalador y ejecútalo en tu computadora.

![alt text](image-2.png)

3. Habilita la casilla de verificación en Install launcher for all users y Add Python 3.8 to PATH. A continuación presiona en Install Now. Windows te solicitará permisos para instalar Python en tu computadora.

![alt text](image-3.png)

4. Al finalizar la instalación se abrirá una ventana como la siguiente, en ella deberás presionar en la opción Disable path length limit. Windows te solicitará permisos para realizar este cambio.

![alt text](image-4.png)

Visual Studio Code
En el curso el profesor utiliza Visual Studio Code, un editor de textos que tiene integradas varias herramientas que te ayudarán a desarrollar tus ejercicios con facilidad. Para obtenerlo en tu computadora, dirígete a: <https://code.visualstudio.com/>

![alt text](image-5.png)

1. Realiza una instalación normal de Visual Studio code.

![alt text](image-6.png)

Una vez instalado se ejecutará Visual Studio Code.

2. En Visual Studio Code dirígete al panel de Extensiones, se encuentra en el panel lateral izquierdo. Ahí deberás buscar la extensión llamada Python.

![alt text](image-7.png)

3. Selecciona la extensión creada por Microsoft, la identificarás por ser similar a la que se muestra en la imágen. Una vez seleccionada, instálala

![alt text](image-8.png)

4. Una vez instalada, reinicia Visual Studio Code.
Listo con esto podrás correr los programas que escribas en python en la terminal de Visual Studio Code.

Cuando quieras correr tu programa en la terminal de Visual Studio Code, puedes introducir la dirección como lo muestra el profesor en el curso o presionar en el botón “Run Python File in Terminal”

![alt text](image-9.png)

Para este caso en particular tengo instalado WSL Ubuntu

### Elementos básicos de Python

Lenguajes de programación

* Bajo nivel vs. alto nivel

* General vs. dominio específico

* Interpretado vs. compilado

**¿Qué es un lenguaje de programación?** Es un lenguaje formal que, mediante una serie de instrucciones, le permite a un programador escribir un conjunto de órdenes, acciones consecutivas, datos y algoritmos para, de esa forma, crear programas que controlen el comportamiento físico y lógico de una máquina.

**¿Qué tipos de lenguaje de programación existen?** El lenguaje de programación es la base para construir todas las aplicaciones digitales que se utilizan en el día a día y se clasifican en dos tipos principales: lenguaje de bajo nivel y de alto nivel.

Lenguaje de programación de bajo nivel Son lenguajes totalmente orientados a la máquina. Este lenguaje sirve de interfaz y crea un vínculo inseparable entre el hardware y el software.

Lenguaje de programación de alto nivel Tienen como objetivo facilitar el trabajo del programador, ya que utilizan unas instrucciones más fáciles de entender.

Lenguaje específico de dominio En desarrollo de software e ingeniería de dominio, un lenguaje específico de dominio, o "lenguaje específico del dominio", (en inglés domain-specific language, DSL) es un lenguaje de programación o especificación dedicado a resolver un problema en particular, representar un problema específico y proveer una técnica para solucionar una situación particular. El concepto no es nuevo pero se ha vuelto más popular debido al aumento del uso de modelaje específico del dominio.1​

Lenguaje de propósito general Se llama lenguaje de propósito general al lenguaje de programación cuyos procedimientos, instrucciones y estructuras de datos están diseñados para resolver todo tipo de problemas.

Lenguaje de interpretados y compilados La principal diferencia entre un lenguaje compilado y uno interpretado es que el lenguaje compilado requiere un paso adicional antes de ser ejecutado, la compilación, que convierte el código que escribes a lenguaje de máquina. Un lenguaje interpretado, por otro lado, es convertido a lenguaje de máquina a medida que es ejecutado.

Ejemplos de lenguajes compilados incluyen C, C++, Java, Go y Rust, entre muchos otros. Ejemplos de lenguajes interpretados incluyen Ruby, Python y JavaScript, entre muchos otros. A todos estos lenguajes se les conoce como lenguajes de alto nivel.

```py
1 + 1 # 1
'Platzi' / 5 # Error
'Platzi' * 3 #PlatziPlatziPlatzi
#PrintStatement
print('Hola mundo')
'Mr' + '. Internatuta'
2 + 2
```

**¿Que es un objeto?** Concepto, abstracción o cosa con límites bien definidos y con significado para el problema que se está manejando

* Escalares vs No escalares -Tipos int. float. bool. str.

```py
#Definiendo variables
my_int  = 1
my_float = 1.0
my_bool = True
my_none = None
my_str = 'Hola'
```

```py
#Imprimiendo el tipo
type(my_int)
type(my_float)
type(my_bool)
type(my_none)
type(my_str)
```

**¿Que pasa si ejecutas esto?**

```py
1 + 1 
2 - 5
2.0 * 3
6 // 2
6 // 4
6 / 4
7 % 2
2 ** 2
```

Resultado

```py
>>> 1 + 1
2
>>> 2 - 5
-3
>>> 2.0 * 3
6.0
>>> 6 // 2
3
>>> 6 // 4
1
>>> 6 / 4
1.5
>>> 7 % 2
1
>>> 2 ** 2
```

![alt text](image-10.png)

![alt text](image-11.png)

![alt text](image-12.png)

### Asignación de variables

![alt text](image-13.png)

Corregir definicion de variables

![alt text](image-14.png)

Reasignacion de memoria

![alt text](image-15.png)

![alt text](image-16.png)

**Un recolector de basura (del inglés garbage collector)** es un mecanismo implícito de gestión de memoria implementado en algunos lenguajes de programación de tipo interpretado o semiinterpretado.

**Variables**

* Pueden contener mayúsculas, minúsculas, números (sin comenzar con uno) y el símbolo _
* No pueden llamarse como las palabras reservadas

![alt text](image-17.png)

* Hacen los programas más comprensibles.
* Son simplemente nombres que apuntan a un valor en memoria.
* El operador de asignación (=) asocia una variable con un valor.

### Cadenas y entradas

![alt text](image-18.png)

![alt text](image-19.png)

![alt text](image-20.png)

![alt text](image-21.png)

![alt text](image-22.png)

Cadenas (strings)

* Los objetos de tipo str pueden representarse con “ ” o ‘ ’.
* El operador + tiene diferente significado según el tipo de dato (overloaded). Con cadenas significa concatenación.
* El operador * es el operador de repetición con cadenas.
* Las cadenas son inmutables.

Entradas (inputs)

* Python tiene la función input para recibir datos del usuario del programa.
* Input siempre regresa cadenas, por lo que si queremos utilizar otro tipo, tenemos que hacer type casting.

![alt text](image-23.png)

![alt text](image-24.png)

![alt text](image-25.png)

### Programas ramificados

```sh
>>> 2 == 3
>>> 2 != 3
>>> 2 > 3
>>> 2 < 3
>>> 2 <= 3
>>> 2 >= 3
```

```sh
>>> True and True
>>> False or True
>>> not True
```

![alt text](image-26.png)

![alt text](image-27.png)

```sh
print("Bienvenido al comparador de edades.")
print("Ahora descubriremos juntos quien tiene mas edad entre dos personas.")
print("Para esto necesitare que me brindes información antes (Soy una computadora, no una adivina... por ahora...)")

nombre_persona_1 = input("Necesito el nombre de la primer persona. ¿Como se llama?: ")
edad_persona_1 = int( input("¿Que edad tiene?: "))
nombre_persona_2 = input("Necesito el nombre de la segunda persona. ¿Como se llama?: ")
edad_persona_2 = int( input("¿Que edad tiene?: "))

print("Despejare la incertidumbre...")

if edad_persona_1 > edad_persona_2:
    print(f"Claro como el agua, {nombre_persona_1} es mayor que {nombre_persona_2}.")
elif edad_persona_1 < edad_persona_2:
    print(f"¡Elemental Watson!, {nombre_persona_2} es mayor que {nombre_persona_1}.")
else:
    print(f"¡Basta de contiendas {nombre_persona_1} y {nombre_persona_2}, ambos tienen la misma edad!")

print("Gracias por usar este programa. ¡Nos vemos la proxima!")
```
