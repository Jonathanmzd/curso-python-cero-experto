# Indice

## ¿Ya tomaste el Curso de Pensamiento Computacional?

**Objetivos**

* Entender cómo funciona la Programación Orientada a Objetos.
* Entender cómo medir la eficiencia temporal y espacial de nuestros algoritmos.
* Entender cómo y por qué graficar.
* Aprender a resolver problemas de búsqueda, ordenación y optimización.

## Introducción a la complejidad algorítmica

* ¿Por qué comparamos la eficiencia de un algoritmo?
* Complejidad temporal vs complejidad espacial
* Podemos definirla como T(n)

**Aproximaciones**

* Cronometrar el tiempo en el que corre un algoritmo.
* Contar los pasos con una medida abstracta de operación.
* Contar los pasos conforme nos aproximamos al infinito.

A continuación te dejo el código con una corrección en el returnde la función recursiva:

```sh
import time

def factorial(n):
    respuesta = 1

    while n > 1:
        respuesta *= n
        n -= 1

    return respuesta


def factorial_r(n):
    if n == 1:
        return 1

    return n * factorial_r(n - 1)


if __name__ == '__main__':
    n = 200000

    comienzo = time.time()
    factorial(n)
    final = time.time()
    print(final - comienzo)

    comienzo = time.time()
    factorial_r(n)
    final = time.time()
    print(final - comienzo)
```

## Abstracción

![alt text](image.png)
