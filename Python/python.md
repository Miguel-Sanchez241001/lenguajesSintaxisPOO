
# Iinicio

Material util para no olvidar sintaxis de python
incluye material usado con frecuencia actualmente.

## Contenido

- [Iinicio](#iinicio)
  - [Contenido](#contenido)
  - [Tipos de datos](#tipos-de-datos)
    - [Numericos](#numericos)
    - [Booleanos](#booleanos)
    - [Cadenas de texto](#cadenas-de-texto)
  - [Funcion util](#funcion-util)
  - [Operadores basicos](#operadores-basicos)
  - [Operadores a nivel de bits](#operadores-a-nivel-de-bits)
  - [Operadores logicos](#operadores-logicos)
  - [Estrutucturas de condiciones](#estrutucturas-de-condiciones)
  - [Estrucutra de bucles](#estrucutra-de-bucles)
  - [Lista,Tuplas,diccionarios](#listatuplasdiccionarios)
    - [Lista](#lista)
    - [tupla](#tupla)
    - [diccionario](#diccionario)
  - [Funciones](#funciones)

## Tipos de datos

- Existiran mas tipos de datos pero estos son los que uso por el momento a medida q los conozco ire agregando

### Numericos

- **int**
- **float**

```python
soyEntero = 10

soyFloat = 24.5
```

---

[👆](#contenido)

### Booleanos

```python
# cualquier valor numerico diferente de 0 
# e considera verdadero si esta en una condicina
soyVerdad = True
# valores iguales a 0 considerados falso
soyMentira = False
```

---

[👆](#contenido)

### Cadenas de texto

- Como lo veo no interesa las comilas aunque si quieres q tu mensje tenga comillas, si

```python
soyUnString = 'pablito'

soyUnStringConComillas = " \"tengo comillas\""
# multiplicar cadenas de texto
soyUnString = 'a'*3 # aaa
```

---

[👆](#contenido)

## Funcion util

- Para concer el tipo de dato de cualquier variable o resultado de un funcion
- Para imprimir texto en pantalla

```python
x = 10
print(type(x))
# esto arroja int
# sep: parametro para el separador
# end parametro para el final
print('yo me','por el sep',sep='uno',end='y termino con el end')
```

[👆](#contenido)

## Operadores basicos

```python
  # mismo + , - , * , / , //,%,**
 # division entera //
 a = 10//3 # 3
 # potencia
 b = 10**3 # 1000
```

[👆](#contenido)

## Operadores a nivel de bits

```python
# ~,|,&,^,<<,>>
a = 7 #---> 111
# ~a ---> -8
# a | 5 --> 7
# a &  5 --> 5
# a ^ 5 --> 2
# a >> 2 --> 1
# a << 2 --> 28
```

[👆](#contenido)

## Operadores logicos

```python
a = 10 > 5 and 5*2 <=10 # True
b = not a # False 
c = a or b # True
```

[👆](#contenido)

## Estrutucturas de condiciones

```python
# if
if not a % 10:
  print("es multiplo de 10")
# elif
elif not a % 3:
  print('a es multiplo de 3')
# else
else:
  print('a no es multiplo de 10 y de 3')
```

[👆](#contenido)

## Estrucutra de bucles

- while
  
```python
while True:
  print("corriendo una ves")
  break # continue
else:
  print('salgo al final del ciclo')
```

[👆](#contenido)

- for
  
```python

for i in range(10):
    i=i - 10
    print(i)
 
else:
    print('ultimo valor de i',i)
```

[👆](#contenido)

## Lista,Tuplas,diccionarios

[Revisar la siguente info](https://docs.hektorprofe.net/python/metodos-de-las-colecciones/metodos-de-las-listas/)

### Lista
  
```python
lts  = [] # lista vacia

lts = [x for x in range(10)] # de 0 al 9 
del lts[0]

lts.sort() # ordena
lts.reverse() # invierte el orden
lts.clear() # limpia
len(tupla) # dimension de la lista
tupla.count(5) # numero de repeticiones del elemento
lts2 = lts.copy() # copia lista
```

[👆](#contenido)

### tupla
  
```python
tupla  = (1,2,8,6) # lista vacia
# objeto inmutable
len(tupla) # dimension de la lista
tupla.count(5) # numero de repeticiones del elemento
tupla.index(6)
```

[👆](#contenido)

### diccionario
  
```python
dic  = {'uno':1,'dos':2,'tres':3} 

for clave, valor in dic.items():
    print(clave, valor)
# uno 1
# dos 2
# tres 3

```

[👆](#contenido)

## Funciones
  
```python
def saludo(men = 'hola soy ',nom=" persona"):
    
    return men + nom

print(saludo(nom="juan"))

print(saludo("juan es"))
```

[👆](#contenido)