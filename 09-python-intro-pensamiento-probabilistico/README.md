# Indice

## Curso de Introducción al Pensamiento Probabilístico - 09-python-intro-pensamiento-probabilistico

La programación probabilística es una herramienta utilizada para crear modelos estadísticos, y realizar inferencias sobre dichos modelos. Aprender las bases te permitirá desarrollar habilidades para dominar lenguajes y librerías especializadas en ejecutar cómputos, como Pyro de Uber, un lenguaje de programación para hacer Inteligencia Artificial.

### Introducción a la programación probabilística

* La programación probabilística utiliza probabilidades y modelos probabilísticos para ejecutar cómputos.
* Se utiliza en una gran cantidad de campos: investigación científica, inteligencia artificial, medicina, etc.
* Existen lenguajes y librerías especializadas para ejecutar este tipo de cómputo, como Pyro de Uber.

![alt text](image.png)

### Probabilidad condicional

La probabilidad condicional es la probabilidad de que ocurra un evento A, sabiendo que también sucede otro evento B. La probabilidad condicional se escribe P(A|B), y se lee «la probabilidad de A dado B».

No tiene por qué haber una relación causal o temporal entre A y B. A puede preceder en el tiempo a B, sucederlo o pueden ocurrir simultáneamente. A puede causar B, viceversa o pueden no tener relación causal. Las relaciones causales o temporales son nociones que no pertenecen al ámbito de la probabilidad. Pueden desempeñar un papel o no, dependiendo de la interpretación que se le dé a los eventos.

La notación para escribir,

«la probabilidad de A y B suceden»: ![alt text](image-1.png)

«la probabilidad de B»: ![alt text](image-2.png)

Un ejemplo de esto puede ser la probabilidad que una persona tenga cáncer, luego de realizar pruebas.

![alt text](image-3.png)

Otro ejemplo es cual es la probabilidad de que una persona use drogas, pero como dato adicional esta persona es músico.

![alt text](image-4.png)

### Teorema de Bayes

El teorema de Bayes, en la teoría de la probabilidad, es una proposición planteada por el matemático inglés Thomas Bayes (1702-1761)​ y publicada póstumamente en 1763,​ que expresa la probabilidad condicional de un evento aleatorio A dado B en términos de la distribución de probabilidad condicional del evento B dado A y la distribución de probabilidad marginal de solo A.

En términos más generales y menos matemáticos, el teorema de Bayes es de enorme relevancia puesto que vincula la probabilidad de A dado B con la probabilidad de B dado A. Es decir, por ejemplo, que sabiendo la probabilidad de tener un dolor de cabeza dado que se tiene gripe, se podría saber (si se tiene algún dato más), la probabilidad de tener gripe si se tiene un dolor de cabeza. Muestra este sencillo ejemplo la alta relevancia del teorema en cuestión para la ciencia en todas sus ramas, puesto que tiene vinculación íntima con la comprensión de la probabilidad de aspectos causales dados los efectos observados.

Sea ![alt text](image-5.png) un conjunto de sucesos mutuamente excluyentes y exhaustivos, y tales que la probabilidad de cada uno de ellos es distinta de cero (0). Sea B un suceso cualquiera del que se conocen las probabilidades condicionales ![alt text](image-6.png). Entonces, la probabilidad ![alt text](image-7.png) viene dada por la expresión:

![alt text](image-8.png)

donde:

* ![alt text](image-9.png) son las probabilidades a priori,
* ![alt text](image-10.png) es la probabilidad de B en la hipótesis A,
* ![alt text](image-11.png) son las probabilidades a posteriori.

Como sabemos que ![alt text](image-12.png) podemos reemplazarlo en la ecuación y nos quedaría:

![alt text](image-13.png)

En este  <https://www.youtube.com/watch?v=HZGCoVF3YvM&t> (en inglés) podras encontrar un video práctico sobre el Teorema de Bayes.

### Análisis de síntomas

En el siguiente ejercicio implementaremos la posibilidad de tener síntomas dado a que una persona tenga cáncer.

![alt text](image-14.png)

```py
# Implementamos la P(B) = P(A)P(B|A) + P(¬A)P(B|¬A)
def prob_b(prob_a, prob_b_dado_a, prob_b_complemento_a):
    calculo = prob_a * prob_b_dado_a + (1-prob_a) * prob_b_complemento_a
    return calculo

# Implementamos la P(A|B) = P(B|A)P(A) / P(B)
def cal_bayes(prob_a, prob_b_dado_a, prob_b_complemento_a):
    prob_evento = prob_b(prob_a, prob_b_dado_a, prob_b_complemento_a)
    calculo = (prob_b_dado_a * prob_a)/prob_evento

    return calculo

if __name__ == "__main__":
    prob_cancer = 1 / 100000
    prob_sintoma_dado_cancer = 1
    prob_sintoma_dado_no_cancer = 10 / 99999
    
    resultado = cal_bayes(prob_cancer, prob_sintoma_dado_cancer, prob_sintoma_dado_no_cancer)

    print(resultado)
```

Vamos a la consola y ejecutamos nuestro programa.

```py
python3 sintomas.py # Ejecutamos nuestro programa

# Y este sera nuestro resultado.
0.09090909090909091
```
