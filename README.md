# Repo4

# 1.Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
```
def es_ascii_vocal_minuscula(numero):
    # Verificar si el número corresponde al código ASCII de una vocal minúscula
    if 97 <= numero <= 122 and chr(numero) in 'aeiou':
        return True
    else:
        return False

# Ejemplos de uso
numero_1 = 97
numero_2 = 105
numero_3 = 120

print(f"{numero_1} es vocal minúscula: {es_ascii_vocal_minuscula(numero_1)}")
print(f"{numero_2} es vocal minúscula: {es_ascii_vocal_minuscula(numero_2)}")
print(f"{numero_3} es vocal minúscula: {es_ascii_vocal_minuscula(numero_3)}")

```
# 2. Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```
def es_codigo_ascii_par(cadena):
    if len(cadena) == 1 and ord(cadena[0]) % 2 == 0:
        return True
    else:
        return False

# Uso
cadena_1 = 'A'
cadena_2 = 'Z'
cadena_3 = 'X'

print(f"El código ASCII de la primera letra de '{cadena_1}' es par: {es_codigo_ascii_par(cadena_1)}")
print(f"El código ASCII de la primera letra de '{cadena_2}' es par: {es_codigo_ascii_par(cadena_2)}")
print(f"El código ASCII de la primera letra de '{cadena_3}' es par: {es_codigo_ascii_par(cadena_3)}")
```

# 3.Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```
def es_digito(caracter):
    
    if caracter.isdigit():
        return True
    else:
        return False

# Uso
caracter_1 = '5'
caracter_2 = 'a'
caracter_3 = '!'

print(f"¿'{caracter_1}' es un dígito?: {es_digito(caracter_1)}")
print(f"¿'{caracter_2}' es un dígito?: {es_digito(caracter_2)}")
print(f"¿'{caracter_3}' es un dígito?: {es_digito(caracter_3)}")
```

#  4. Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:
Positivo: "El número x es positivo"
Negativo: "El número x es negativo"
Cero (0): "El número x es el neutro para la suma"
Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```
import math

def punto_en_circulo(x, y, centro_x, centro_y, radio):
    distancia_al_centro = math.sqrt((x - centro_x)**2 + (y - centro_y)**2)

    if distancia_al_centro < radio:
        print(f"El punto ({x}, {y}) está en el interior del círculo.")
    else:
        print(f"El punto ({x}, {y}) no está en el interior del círculo.")

# Uso:
centro_x = 1
centro_y = 0
radio = 12

punto_en_circulo(3, 4, centro_x, centro_y, radio)
punto_en_circulo(-2, -2, centro_x, centro_y, radio)

```

#  5. Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```
def es_triangulo(a, b, c):
    if a + b > c and a + c > b and b + c > a:
        print("Con estas longitudes se puede construir un triángulo.")
    else:
        print("Con estas longitudes no se puede construir un triángulo.")

# Uso:
longitud_1 = 3
longitud_2 = 4
longitud_3 = 5

es_triangulo(longitud_1, longitud_2, longitud_3)

longitud_4 = 1
longitud_5 = 2
longitud_6 = 7

es_triangulo(longitud_4, longitud_5, longitud_6)

```
