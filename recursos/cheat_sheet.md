# 📋 Python Cheat Sheet - Referencia rápida

## Variables y Tipos

```python
# Strings
nombre = "Python"
print(f"Hola {nombre}")

# Números
entero = 42
float_num = 3.14

# Booleanos
activo = True
inactivo = False

# Conversiones
str(42)      # "42"
int("42")    # 42
float("3.14") # 3.14
```

## Listas

```python
lista = [1, 2, 3, 4, 5]
lista[0]           # 1
lista[-1]          # 5
lista[1:3]         # [2, 3]
lista.append(6)    # [1, 2, 3, 4, 5, 6]
lista.pop()        # Elimina el último
len(lista)         # Longitud
```

## Diccionarios

```python
persona = {
    "nombre": "Juan",
    "edad": 30,
    "ciudad": "Madrid"
}

persona["nombre"]           # "Juan"
persona.keys()              # dict_keys([...])
persona.values()            # dict_values([...])
persona.get("edad")         # 30
persona["pais"] = "España"  # Añadir nueva clave
```

## Condicionales

```python
if edad >= 18:
    print("Mayor de edad")
elif edad >= 13:
    print("Adolescente")
else:
    print("Menor")

# Operador ternario
estado = "activo" if estado_bool else "inactivo"
```

## Bucles

```python
# For
for i in range(5):
    print(i)  # 0, 1, 2, 3, 4

# For con lista
for elemento in [1, 2, 3]:
    print(elemento)

# While
contador = 0
while contador < 5:
    print(contador)
    contador += 1

# Enumerate
for indice, valor in enumerate(["a", "b", "c"]):
    print(indice, valor)  # 0 a, 1 b, 2 c
```

## Funciones

```python
def saludar(nombre, apellido=""):
    return f"Hola {nombre} {apellido}"

saludar("Juan")                      # "Hola Juan "
saludar("Juan", "Pérez")            # "Hola Juan Pérez"

# Lambda
cuadrado = lambda x: x ** 2
cuadrado(5)  # 25
```

## Comprensiones

```python
# List comprehension
cuadrados = [x**2 for x in range(5)]  # [0, 1, 4, 9, 16]

# Con condición
pares = [x for x in range(10) if x % 2 == 0]  # [0, 2, 4, 6, 8]

# Dict comprehension
dict_cuadrados = {x: x**2 for x in range(5)}
```

## Strings

```python
text = "Hola Python"

text.upper()           # "HOLA PYTHON"
text.lower()           # "hola python"
text.replace("Hola", "Hi")  # "Hi Python"
text.split()           # ["Hola", "Python"]
" ".join(["Hola", "Python"])  # "Hola Python"
len(text)              # 11
"Python" in text       # True
```

## Manejo de Errores

```python
try:
    resultado = 10 / 0
except ZeroDivisionError:
    print("No se puede dividir entre cero")
except Exception as e:
    print(f"Error: {e}")
finally:
    print("Siempre se ejecuta")
```

## Archivos

```python
# Lectura
with open("archivo.txt", "r") as f:
    contenido = f.read()
    # contenido = f.readlines()  # Lista de líneas

# Escritura
with open("archivo.txt", "w") as f:
    f.write("Contenido nuevo")

# Añadir
with open("archivo.txt", "a") as f:
    f.write("\nMás contenido")
```

## Clases

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def saludar(self):
        return f"Hola, soy {self.nombre}"

persona = Persona("Juan", 30)
persona.saludar()  # "Hola, soy Juan"
```

## Módulos comunes

```python
import os
import sys
import json
import re
import datetime
import random
import math

# Uso
os.getcwd()          # Directorio actual
sys.version          # Versión de Python
random.randint(1, 10)  # Número aleatorio
math.pi              # 3.14159...
```

---

🔗 Para más info: [docs.python.org](https://docs.python.org/es/3/)
