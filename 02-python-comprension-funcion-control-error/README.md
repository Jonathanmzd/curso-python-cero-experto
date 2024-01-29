## Curso de Python: Comprehensions, Funciones y Manejo de Errores

### El Zen de Python

![Alt text](image.png)

![Alt text](image-1.png)


#### Recursos

https://static.platzi.com/media/public/uploads/slides-del-curso-de-python-comprehensions-funciones-y-manejo-de-errores_d4ad1632-4a52-4a5b-b74e-5a972a02c404.pdf

https://es.wikipedia.org/wiki/Zen_de_Python


### Sets

* Se pueden modificar
* No tienen un orden
* No pueden tener elementos duplicados

![Alt text](image-2.png)

```py
set_countries = {'col', 'mex', 'bol'}
print(set_countries)
print(type(set_countries))

set_numbers = {1, 2, 2, 443, 23}
print(set_numbers)

set_types = {1, 'hola', False, 12.12}
print(set_types)

set_from_string = set('hoola')
print(set_from_string)

set_from_tuples = set(('abc', 'cbv', 'as', 'abc'))
print(set_from_tuples)

numbers = [1,2,3,1,2,3,4]
set_numbers = set(numbers)
print(set_numbers)
unique_numbers = list(set_numbers)
print(unique_numbers)
```

#### Recursos

https://static.platzi.com/media/public/uploads/01_sets_4c6e5f1b-a0b1-46d5-879f-39f81a2119dc.py

https://www.w3schools.com/python/python_sets.asp


### Modificando conjuntos

* add(): Añade un elemento.

* update(): Añade cualquier tipo de objeto iterable como: listas, tuplas.

* discard(): Elimina un elemento y si ya existe no lanza ningún error.

* remove(): Elimina un elemento y si este no existe lanza el error “keyError”.

* pop(): Nos devuelve un elemento aleatorio y lo elimina y si el conjunto está vacío lanza el error “key error”.

* clear(): Elimina todo el contenido del conjunto.


![Alt text](image-3.png)

```py
set_countries = {'col', 'mex', 'bol'}

size = len(set_countries)
print(size)

print('col' in set_countries)
print('pe' in set_countries)

# add
set_countries.add('pe')
print(set_countries)
set_countries.add('pe')
print(set_countries)

# update
set_countries.update({'ar', 'ecua', 'pe'})
print(set_countries)

# remove

set_countries.remove('col')
print(set_countries)

set_countries.remove('ar')
set_countries.discard('arg')
print(set_countries)
set_countries.add('arg')
print(set_countries)
set_countries.clear()
print(set_countries)
print(len(set_countries))
```

#### Recursos

https://static.platzi.com/media/public/uploads/02_crud_set_53ad34c2-4b27-4618-a875-315add8a0e71.py


### Operaciones con conjuntos

**union(set)**: Realiza la operacion “union” entre dos conjuntos. La unión entre dos conjuntos es sumar los elementos de estos sin repetir elementos. Esta operación tambien se puede realizar con el signo “|”: set_a | set_b.

**intersection(set)**: Realiza la operacion “intersection” entre dos conjuntos. La intersección entre dos conjuntos es tomar unicamente los elementos en común de los conjutnos. Esta operación tambien se puede realizar con el signo “&”: set_a & set_b.

**difference(set)**: Realiza la operacion “difference” entre dos conjuntos. La diferencia entre dos conjuntos es restar los elementos del segundo conjunto al primero. Esta operación tambien se puede realizar con el signo “-”: set_a - set_b.

**symmetric_difference(set)**: Realiza la operacion “symmetric_difference” entre dos conjuntos. La diferencia simetrica entre dos conjutnos consta de restar todos los elementos de ambos exceptuando el elemento en común. Esta operación tambien se puede realizar con el signo “^”: set_a ^ set_b.

![Alt text](image-4.png)

```py
set_a = {'col', 'mex', 'bol'}
set_b = {'pe', 'bol'}

set_c = set_a.union(set_b)
print(set_c)
print(set_a | set_b)

set_c = set_a.intersection(set_b)
print(set_c)
print(set_a & set_b)

set_c = set_a.difference(set_b)
print(set_c)
print(set_a - set_b)

set_c = set_a.symmetric_difference(set_b)
print(set_c)
print(set_a ^ set_b)
```

#### Recursos

https://static.platzi.com/media/public/uploads/03_operations_f46bef8b-d2a2-4da1-9806-a9271df1954d.py

https://www.w3schools.com/python/python_ref_set.asp


### List Comprehension

![Alt text](image-5.png)

![Alt text](image-6.png)

![Alt text](image-7.png)

![Alt text](image-8.png)

![Alt text](image-9.png)

```py
'''
numbers = []
for element in range(1, 11):
  numbers.append(element * 2)

print(numbers)

numbers_v2 = [element * 2 for element in range(1, 11)]
print(numbers_v2)
'''
numbers = []
for i in range(1, 11):
  if i % 2 == 0:
    numbers.append(i * 2)

print(numbers)

numbers_v2 = [i * 2 for i in range(1, 11) if i % 2 == 0]
print(numbers_v2)
```

#### Recursos

https://static.platzi.com/media/public/uploads/04_lists_54fe02b6-b356-41cd-8e4d-05f0154686be.py

https://www.w3schools.com/python/python_lists_comprehension.asp

### Dictionary Comprehension

![Alt text](image-10.png)

![Alt text](image-11.png)

```py
'''
dict = {}
for i in range(1, 5):
  dict[i] = i * 2

print(dict)

dict_v2 = { i: i * 2 for i in range(1, 5)}
print(dict_v2)

import random
countries = ['col', 'mex', 'bol', 'pe']
population = {}
for country in countries:
  population[country] = random.randint(1, 100)

print(population)

population_v2 = { country: random.randint(1, 100)  for country in countries}
print(population_v2)
'''
names = ['nico', 'zule', 'santi']
ages = [12, 56, 98]

print(list(zip(names, ages)))

new_dict = {name: age for (name, age) in zip(names, ages)}
print(new_dict)
```

#### Recursos

https://static.platzi.com/media/public/uploads/05_dict_c61ed7f9-deb7-41b8-984d-be47d893676a.py