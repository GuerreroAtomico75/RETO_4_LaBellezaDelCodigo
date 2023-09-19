# RETO_4_LaBellezaDelCodigo
### Importante:
##### La descripción completa del Reto 4 está al principio de esta repo, en el archivo REPO_4_NOTEBOOK.ipynb. Lo recomendable es que usted pueda detallar esta repo desde ese archivo, pero si por algún motivo lo quiere ver desde este README también lo puede hacer, teniendo en cuenta que se mostrara el enunciado del problema y la solución del  problema, pero SIN la descripcón de lo que fue solucionar el problema y que se tuvo en cuenta a la hora se solucionarlo; también tener en cuenta para mayor facilidad (desde mi humilde e ignorante punto de vista) al usted mirar el archivo desde el notebook tendrá la opción de ir al mismo Google Collab para poder correr los ejercicio. Sin mucha más información. Muchas Gracias

---

### Problemas planteados (con su respectiva solución):
1. ##### Dado un número entero, determinar si ese número corresponde al código ASCII de una vocal minúscula.
```
#Se declara variable
n : int
#Inicializo variable, pidiendo que se ingrese un numero entero
n = int(input("Ingrese un numero entero el cual pertenezca en codigo ASCII a una vocal minuscula: "))
if n == 97 or n == 101 or n == 105 or n == 111 or n == 117:
    print("El numero ingresado pertenece en codigo ASCII a una vocal minuscula")
    print("La vocal minuscula es", chr(n))
else:
    print("El numero ingresado no pertenece en codigo ASCII a una vocal minuscula")
```

---

2. ##### Dada una cadena de longitud 1, determine si el código ASCII de primera letra de la cadena es par o no.
```
#Declaramos la variable
car : str
#Inicializamos variable, teniendo en cuenta que la cadena es de una longitud de 1
car = input("Ingrese un solo caracter que puede ser letra, numero o simbolo: ")
cod = ord(car)
#Añadimos condicional
if cod % 2 == 0:
    print("El código ASCII del caracter ingresado es par")
    print(cod)
else:
    print("el código ASCII del caracter ingresado es impar")
    print(cod)
```

---

3. ##### Dado un carácter, construya un programa en Python para determinar si el carácter es un dígito o no.
```
#Inicializamos la variable como un caracter que se va a ingresar
n = (input("ingrese un caracter: "))
#Condicionamos el caracter ingresado con .isdigit()
if n.isdigit():
    print(n, "es un digito")
else:
    print(n, "no es un digito")
```

---

4. ##### Dado un número real x, construya un programa que permita determinar si el número es positivo, negativo o cero. Para cada caso de debe imprimir el texto que se especifica a continuación:
* Positivo: "El número x es positivo"
* Negativo: "El número x es negativo"
* Cero (0): "El número x es el neutro para la suma"
```
#Declaramos la variable
x : float
# Inicializamos
x = float(input("ingrese un número real cualquiera: "))
#Condicionamos
if x > 0:
    print("El numero", x, "es positivo")
elif x < 0:
    print("El numero", x, "es negativo")
elif x==0:
    print("el numero", x, "es el neutro para la suma")
```

---

5. ##### Dado el centro y el radio de un círculo, determinar si un punto de R2 pertenece o no al interior del círculo.
```
#Definimos y declaramos las variables
#Primero las del centro del circulo y su radio
x : float
y : float
r : float
#Despues las del Punto R2
m : float
n : float
#Inicializamos las variables
#Tener en cuenta que el valor de m y n son paralelos al eje "x" y "y" en el plano respectivamente.
m = float(input("ingrese un valor para el punto m: "))
n = float(input("ingrese un valor para el punto n: "))
r = float(input("ingrese un valor para el radio: "))
x = float(input("ingrese un valor para el punto x: "))
y = float(input("ingrese un valor para el punto y: "))
#Condicionamos
if (((m - x)**2) + ((n - y)**2))**0.5 < r:
    print("El punto R2 pertenece al interior del circulo")
else:
    print("El punto R2 no pertenece al interior del circulo")
```

---

6. ##### Dadas tres longitudes positivas, determinar si con esas longitudes se puede construir un triángulo.
```
#Declaramos variables
x : float
y : float
z : float
#Inicializamos las variables
x = float(input("ingresa un valor para la longitud x: "))
y = float(input("ingresa un valor para la longitud y: "))
z = float(input("ingresa un valor para la longitud z: "))
#condicionamos
if x <= z and y <= z:
    if x + y > z:
        print("Se puede construir un triangulo con las longitudes ingresadas")
    else:
        print("No se puede construir un triangulo con las longitudes ingresadas")
elif x <= y and z <= y:
    if x + z > y:
        print("Se puede construir un triangulo con las longitudes ingresadas")
    else:
        print("No se puede construir un triangulo con las longitudes ingresadas")
elif y <= x and z <= x:
    if y + z > x:
        print("Se puede construir un triangulo con las longitudes ingresadas")
    else:
        print("No se puede construir un triangulo con las longitudes ingresadas")
```

---

### Eso es todo, Gracias por ver este Repo. Espero haya sido de su agrado.
*Mario Alejandro Martinez Bedoya*
