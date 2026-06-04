# 1.2 Variables y Tipos de Datos

## ¿Qué es una variable?

Una variable es un contenedor que guarda información.

```python
edad = 20
nombre = "Juan"
activo = True
```

## Tipos de Datos Básicos

### 1. int (Enteros)
```python
edad = 20
port = 8080
print(type(edad))  # <class 'int'>
```

### 2. float (Decimales)
```python
altura = 1.75
pi = 3.14159
print(type(altura))  # <class 'float'>
```

### 3. str (Cadenas de texto)
```python
nombre = "Christian"
ciudad = "Madrid"
print(type(nombre))  # <class 'str'>
```

### 4. bool (Booleanos)
```python
conectado = True
error = False
print(type(conectado))  # <class 'bool'>
```

## Conversión de tipos

```python
# String a int
numero = int("42")

# Int a string
texto = str(25)

# Cualquier cosa a float
decimal = float(10)
```

## Entrada de usuario

```python
nombre = input("¿Cuál es tu nombre? ")
edad = int(input("¿Cuántos años tienes? "))
print(f"Hola {nombre}, tienes {edad} años")
```

## Asignar múltiples variables

```python
a, b, c = 1, 2, 3
x = y = z = 0
```

**Siguiente:** [1.3 Operadores Básicos](./1_3_operadores.md)
