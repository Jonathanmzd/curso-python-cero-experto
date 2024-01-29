## Curso de Fundamentos de Python

Aprende a programar en Python desde cero. Potencia tu futuro con el lenguaje en auge en data science, desarrollo backend, Machine Learning, IoT y más. Crea tus primeros programas utilizando variables, estructuras de datos, condicionales y ciclos.

### ¿Por qué aprender a programar en Python?

1) Python ocupa siempre los primeros puestos de los lenguajes mas queridos.

2) Es fácil de aprender.

3) Esta en el top 20 de los lenguajes de programación mejor pagos.

4) Puede ser utilizado en diferentes áreas, especialmente en Análisis de datos (51%) y desarrollo web (45%).

5) Tiene una demanda laboral muy grande en el mundo de la tecnología.

#### Recursos

https://insights.stackoverflow.com/survey/2021

https://www.jetbrains.com/lp/devecosystem-2021/


### Herramientas del curso

![Alt text](image.png)

#### Recursos

https://replit.com/

https://replit.com/@nicobytes/Python101?v=1#01_print.py

###  Tu primer programa con Python

Tener cuidado con la identacion 

```py
print("Hola, esto es el archivo 01")

print("Hola soy Nicolas y tengo 12 aÃ±os")

# operaciones...

print(12 + 5)
print(10 - 5)
print(2 * 3)
print(8 / 2)

# Esto es un comentario
"""
varias
lineas
otra
"""
'''
varias 
lienas
'''
```

#### Recursos

https://replit.com/@nicobytes/Python101?v=1#01_print.py

https://replit.com/@NicolasMolina13/Python-101

### Herramientas para programar con Python

¡Hola, te doy la bienvenida a esta clase con un mensaje muy especial!

![Alt text](image-1.png)

En este curso, gracias a la herramienta de Replit, NO tienes que instalar nada en tu computador para comenzar a programar. Pero te tengo un mensaje del futuro muy importante: en tu día a día programando utilizarás otras herramientas que te permitirán construir software de manera profesional.

Algunas de estas herramientas son las siguientes:

* Editores de código como Visual Studio Code.
* Terminal y línea de comandos en diversos sistemas operativos.
* Jupyter Notebooks (si decides entrar a data science).
* Git para control de versiones.
* Entornos virtuales con PIP.
* Entornos integrados de desarrollo (IDE) como PyCharm, Visual Studio o DataSpell.
  
![Alt text](image-2.png)

Por ahora NO nos preocuparemos por todo esto, ni por alguna instalación. Lo más importante en este momento que estás dando tus primeros pasos es que aprendas los fundamentos del lenguaje Python.

En cursos posteriores de la ruta de aprendizaje que sigues, instalarás y conocerás herramientas que te permitirán programar con Python de manera profesional.

¡Sigue avanzando en tu ruta de aprendizaje! 🐍💚

### Variables

Para imprimir directamente el archivo desde la terminal lo realizamos de la siguiente manera:

Ingresamos a la shell

```shell
python 02_vars.py
```

Ejercicios

```py
print("Hola, vars")

# esto es una variable
my_name = "Nicolas"
print(my_name)

# esto es variable con un numero
my_age = 12
print(my_age)

my_name = "Santiago"
print("aqui cambio", my_name)

# input

my_name = input("Â¿CuÃ¡l es tu nombre?")
print("usando input", my_name)
```

#### Recursos

https://www.w3schools.com/python/python_variables.asp

### Tipos de datos

Tipos de datos primitivos

* Integers: números Enteros
* Floats: números de punto flotante (decimales)
* Strings: cadena de caracteres (texto)
* Boolean: boolenaos (Verdadero o Falso)
  
Tipos de dato adicionales

* Datos en texto: str
* Datos numéricos: int, float, complex
* Datos en secuencia: list, tuple, range
* Datos de mapeo: dict
* Set Types: set, frozenset
* Datos booleanos: bool
* Datos binarios: bytes, bytearray, memoryview

![Alt text](image-3.png)

```py
# string
my_name = "Nicolas"
my_name = 'Santiago'
my_name = "12"
print('my_name =>', my_name)
print(type(my_name))

# int
my_age = 12
print('my_age =>', my_age)
print(type(my_age))

# boolean
is_single = False
print('is_single =>', is_single)
print(type(is_single))

# inputs
my_age = input('Â¿CuÃ¡l es tu edad? ')
print('my_age =>', my_age)
print(type(my_age))
```

#### Recursos

https://www.w3schools.com/python/python_datatypes.asp


### Strings

![Alt text](image-4.png)

```py
name = "Nicolas"
last_name = 'Molina Monroy'
print(name)
print(last_name)

full_name = name + " " + last_name
print(full_name)

quote = "I'm Nicolas"
print(quote)

quote2 = ' She said "Hello"  '
print(quote2)

# format
template = "Hola, mi nombre es " + name + " y mi apellido es " + last_name
print('v1 ', template)

template = "Hola, mi nombre es {} y mi apellido es {}".format(name, last_name)

print('v2', template)

template = f"Hola, mi nombre es {name} y mi apellido es {last_name}"
print('v3', template)
```

#### Recursos

https://static.platzi.com/media/public/uploads/04_string_463dac54-1e10-4e3f-b621-478f0a13fbef.py