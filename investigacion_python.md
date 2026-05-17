# Investigación sobre Python

## 1. ¿Qué es una variable en Python?

Una variable es un espacio en memoria que se utiliza para almacenar información o datos que pueden cambiar durante la ejecución del programa.

### Tipos de datos que pueden almacenar

- Enteros (int): números sin decimales.
- Strings (str): texto o cadenas de caracteres.
- Flotantes (float): números con decimales.
- Booleanos (bool): valores True o False.

### Ejemplos de nombres válidos

- nombre_usuario
- edad
- totalCompra

### Ejemplos de nombres inválidos

- 1numero
- mi-variable
- class

---

## 2. ¿Qué diferencia hay entre = y == en Python?

- = se utiliza para asignar un valor a una variable.
- == se utiliza para comparar dos valores.

### Ejemplos

```python
edad = 20
Asigna el valor 20 a la variable edad.

edad == 20

Compara si edad es igual a 20.

# 3. ¿Qué es la indentación en Python y por qué es importante?

La indentación es el espacio que se deja al inicio de una línea de código para indicar bloques o estructuras como ciclos, funciones y condicionales.

Es importante porque Python utiliza la indentación para entender la estructura del programa.

## ¿Qué pasa si no indentas correctamente?

El programa genera errores de sintaxis y no puede ejecutarse correctamente.

---

# 4. Diferencia entre ciclo for y ciclo while

- for: se utiliza cuando se conoce cuántas veces se repetirá una acción.
- while: se utiliza cuando una acción debe repetirse mientras una condición sea verdadera.

## ¿Cuándo usarías cada uno?

- Usar for para recorrer listas, rangos o repetir un número definido de veces.
- Usar while cuando no se sabe exactamente cuántas repeticiones habrá.

## Ejemplo de for

```python
for i in range(5):
    print(i)
    contador = 0

while contador < 5:
    print(contador)
    contador += 1

# 5. ¿Qué hace la función range() en Python?

La función `range()` genera una secuencia de números.

## range(5)

Genera números del 0 al 4.

```python
for i in range(5):
    print(i)

range(1, 10)

Genera números del 1 al 9.

for i in range(1, 10):
    print(i)
range(0, 10, 2)

Genera números pares del 0 al 8 avanzando de dos en dos.

for i in range(0, 10, 2):
    print(i)

    
