# Reto_8
1.Imprimir un listado con los números del 1 al 100 cada uno con su respectivo cuadrado.
```python

```

2.Imprimir un listado con los números impares desde 1 hasta 999 y seguidamente otro listado con los números pares desde 2 hasta 1000.
```python

```

3.Imprimir los números pares en forma descendente hasta 2 que son menores o iguales a un número natural n ≥ 2 dado
```python

```

4.Imprimir los números de 1 hasta un número natural n dado, cada uno con su respectivo factorial
```python

```

5.Calcular el valor de 2 elevado a la potencia n usando ciclos for.
```python

```

6.Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for. Disclaimer: Trate de no utilizar el operador de potencia (**).
```python
n = int(input("Digite el valor de n: "))
x = float(input("Digite el valor de x: "))
resultado = 1.0
for _ in range(n):
    resultado *= x
print(f"{x} elevado a la potencia {n} es {resultado}")
```
7.Diseñe un programa que muestre las tablas de multiplicar del 1 al 9.
```python

```

8.Diseñar una función que permita calcular una aproximación de la función exponencial alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Maclaurin. Nota: use math para traer la función exponencial y mostrar la diferencia entre el valor real y la aproximación.

[![image.png](https://i.postimg.cc/brc6HGX7/image.png)](https://postimg.cc/hzsbKtts)
```python
import math

def aprox_exp(x, n):
    suma = 0.0
    for i in range(n + 1):
        suma += x ** i / math.factorial(i)
    return suma
x = float(input("Digite el valor de x para calcular e^x: "))
n = int(input("Digite el numero de terminos n para la aproximacion: "))
aprox = aprox_exp(x, n)
valor_real = math.exp(x)
print(f"Aprox de e^{x} usando {n} terminos: {aprox}")
print(f"Valor real de e^{x}: {valor_real}")
print(f"Diferencia: {abs(valor_real - aprox)}")
```
9.Diseñar una función que permita calcular una aproximación de la función seno alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Maclaurin. Nota: use math para traer la función seno y mostrar la diferencia entre el valor real y la aproximación.

[![image.png](https://i.postimg.cc/v8rXwZwm/image.png)](https://postimg.cc/MXG1yxTk)

```python

```

10.Diseñar una función que permita calcular una aproximación de la función arcotangente alrededor de 0 para cualquier valor x en el rango [-1, 1], utilizando los primeros n términos de la serie de Maclaurin. Nota: use math para traer la función arctan y mostrar la diferencia entre el valor real y la aproximación.

[![image.png](https://i.postimg.cc/DfBj4NWd/image.png)](https://postimg.cc/jCnQGZ4L)


Disclaimer: Para las aproximaciones de series determine con que valor n se obtiene menos del 0.1% de error.

```python

```
