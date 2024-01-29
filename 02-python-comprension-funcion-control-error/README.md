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