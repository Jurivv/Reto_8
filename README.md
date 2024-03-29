# Reto_8
6.Leer un número natural n, leer otro dato de tipo real x y calcular x^n usando ciclos for. Disclaimer: Trate de no utilizar el operador de potencia (**).
```python
n = int(input("Digite el valor de n: "))
x = float(input("Digite el valor de x: "))
resultado = 1.0
for _ in range(n):
    resultado *= x
print(f"{x} elevado a la potencia {n} es {resultado}")
```
8.Diseñar una función que permita calcular una aproximación de la función exponencial alrededor de 0 para cualquier valor x (real), utilizando los primeros n términos de la serie de Maclaurin. Nota: use math para traer la función exponencial y mostrar la diferencia entre el valor real y la aproximación.
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
