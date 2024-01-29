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

