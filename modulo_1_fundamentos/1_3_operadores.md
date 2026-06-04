# 1.3 Operadores Básicos

## Operadores Aritméticos

```python
a = 10
b = 3

print(a + b)      # 13 (suma)
print(a - b)      # 7 (resta)
print(a * b)      # 30 (multiplicación)
print(a / b)      # 3.333... (división)
print(a // b)     # 3 (división entera)
print(a % b)      # 1 (módulo)
print(a ** b)     # 1000 (potencia)
```

## Operadores de Comparación

```python
print(10 == 10)   # True
print(10 != 5)    # True
print(10 > 5)     # True
print(5 < 10)     # True
print(10 >= 10)   # True
print(5 <= 10)    # True
```

## Operadores Lógicos

```python
# AND - Todos deben ser True
print(True and True)    # True
print(True and False)   # False

# OR - Al menos uno debe ser True
print(True or False)    # True
print(False or False)   # False

# NOT - Niega una condición
print(not False)        # True
print(not True)         # False
```

## Operadores de Asignación

```python
x = 10
x += 5    # x = 15
x -= 3    # x = 12
x *= 2    # x = 24
x /= 4    # x = 6.0
```

## Orden de Operaciones (PEMDAS)

```python
# 1. Paréntesis
# 2. Exponentes
# 3. Multiplicación y División
# 4. Suma y Resta

resultado = 2 + 3 * 4
print(resultado)      # 14 (primero 3*4=12, luego 2+12=14)

resultado = (2 + 3) * 4
print(resultado)      # 20 (primero 2+3=5, luego 5*4=20)
```

**Siguiente:** [1.4 Entrada y Salida de Datos](./1_4_io.md)
