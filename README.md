# PYTHON-MEGACURSO-de-A.D
Hola githubers en esta ocasion he hecho un codigo de python bastante extenso con todo lo necesario que teneis que saber sobre este buen lenguaje de programacion. Podeis copiar y pegar cada uno de los apartados explicados porque ejecutando todo el codigo a la vez va a dar error, la proxima lo hare en modulos separados. En este repositorio vais a ver varios codigos actualizados que ire mejorando poco a poco. Usar el que diga actualizado que viene con mas informacion. Aqui os lo dejo igual:








"""
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
Hola gente de github, he creado este inmenso codigo 
explicando todo lo basico sobre python, espero que 
os sirva de algo, en mi humilde opinion con este codigo
aprendereis mas rapido que con un curso de internet
ya que aqui teneis todo al grano y explicado brevemente
pero respeto vuestra decision. El codigo que he hecho ha sido
a partir de unos apuntes mios de obsidian que hice hace poco, lo he hecho lo mas 
sencillo posible para que no sea demasiado abrumador.
Os aviso de que todo el contenido esta un poco desorganizado,
os encontrareis facilmente cosas basicas al final del todo.
He puesto todo en el mismo script por pereza asi que es muy probable 
que de errores(Lo siento).
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
AUTOR DE ESTE SCRIPT: ALEJANDRO DORAL
"""


#Esto que veis aqui son los imports de momento no le hagais mucho caso,
#import es para traer librerias a nuestro codigo
#En python por convencion se suelen importar
#al principio del codigo pero podeis hacerlo 
#donde querais, por eso python es mi lenguaje favorito...

from random import randint as r
from random import choice as c
from random import shuffle
import datetime
import time
import math
import re
import pandas as pnd
import numpy as np
import matplotlib as mpl
from matplotlib import pyplot as pp
from cryptography.fernet import Fernet
from socket import *
from random import choice as chc
from random import randrange as rndg
import os as os
import statistics
import threading
import time as t
import multiprocessing
import sqlite3
import unittest
from sklearn.linear_model import LinearRegression as ln
from collections import deque as dq
import pickle as pkl
import secrets
import subprocess
import string
import numbers



#Vamos a repasar en este script todo lo basico de python y todo junto.

#0.QUE ES PYTHON          #Autor script: A.D
#Python es un lenguaje de programacion POO(orientada a objetos)
#todo lo que creamos se interpreta como un objeto
#Salio en los años 90 y se caracteriza por su lenguaje facil de entender
#La curva de aprendizaje en python es bastante rapida al principio para los que 
#comienzan en este lenguaje
#Fue creado para parecerse al lenguaje humano que se usa y es bastante sencillo
#Tiene mucha demanda de empleo es el top 1 actual (2024)





#1.LOS PRINTS          #Autor script: A.D
#Este es un print normal y cualquiera
print("No voy a poner Hola mundo")

#El \n se usa para hacer un salto de linea en el print
print("Hola \nbuenas tardes")

#El \t se usa para hacer tabulaciones de cuatro espacios
print("Esto va a ser \ttabulado")

#En otros lenguajes como java se utiliza esto para hacer un print:
#System.out.println("Hi")       python es mas sencillo solo se usa un print()





#2.VARIABLES                 #Autor script: A.D
#Una variable es un contenedor de un valor que le asignemos
#En python no hace falta especificar exactamente 
#el tipo de varible que estamos creando
variable = "Esto es una variable"
mi_variable = 20
mi_variable_suma = 20 + 20 - mi_variable

variable_string = "aaaasfdasdfas"
variable_entero = 234234

#Tenemos que hacer un casting a la variable entero 
#Para que se pueda imprimir en print porque las variables las interpreta
#todas como strings y no puede haber variables de dos tipos distintos
variable_entero = str(variable_entero)
print(variable_string + variable_entero)

#Una variable puede ser tambien una operacion
variable_operacion = 23423 + 234234 -234 *23423423






#3.LOS STRINGS                #Autor script: A.D
#Los strings son un conjunto de cadena de caracteres

String = "Hola"
print(String)

mi_String1 = "Hola"
miString2 = " "
miString3 = "buenas tardes"

#Esto se le llama concatenar
print(mi_String1 + miString2 + miString3)

string_palabra1 = "Ho"
string_palabra2 = "la"
string_palabra_entera = string_palabra1 + string_palabra2
print(string_palabra_entera)






#4.Los inputs                #Autor script: A.D
#Los inputs permiten al usuario ingresar algo en la consola y eso puede ser
#utilizado posteriormente en el codigo del programador

variable_usuario = input("Dime tu nombre por favor ")
variable_usuario2 = input("Dime tu edad " + variable_usuario + " por favor")

print("El nombre del usuario es " + variable_usuario)
print("La edad del usuario es " + variable_usuario2)

print("Dime dos numeros y van a ser sumados")
numero1 = input("Primer numero---> ")
numero2 = input("Segundo numero---> ")
numero1 = int(numero1)
numero2 = int(numero2)
print("Vale has seleccionado: " + str(numero1))
print("Y tambien: " + str(numero2))
print("Vamos a sumarlos...")
suma = numero1 + numero2
print("La suma resultante es: " + str(suma))





# 5. Integers, floats doubles...              #Autor script: A.D

# Un integer es un número entero sin decimales
numero_integer = 100000
numero_float = 1012.123123123123

suma_integer_float = numero_integer + numero_float
print(suma_integer_float)

nuevo_float = 234234234.234234 - 23423.2342
print(nuevo_float)
nuevo_float = nuevo_float + 123123

# En otros lenguajes no podemos sumar integers y floats porque son de distinto tipo
# pero en python sí podemos, es más flexible

# Conversiones
# Una conversión consiste en pasar un tipo de valor a otro que nosotros queramos
# Esto se conoce como casting
# Están las conversiones implícitas y las conversiones explícitas
# Las implícitas se hacen solas
# Las explícitas las hacemos nosotros manualmente

# Estas son las conversiones implícitas, se hacen solas
integer = 10
floattt = 234.32
mezcla = integer + floattt
print(type(mezcla))

# Estas son las conversiones explícitas
floatt = 10.234
floatt = int(floatt)
print(type(floatt))






# 6. Formatear cadenas de texto                    #Autor script: A.D
# Consiste en meter varias variables en una cadena de texto
# y poder por ejemplo imprimirlas

variable_concatenar = "Alex"
oracion = "Mi nombre es "

# La forma normal de formatear sería esta:
print(oracion + variable_concatenar)

# Pero esta es la más cómoda
print(f"{oracion}{variable_concatenar}")

# También se puede hacer con otras variables como integers
numero1 = 1
numero2 = 2
suma = numero1 + numero2
print(f"La suma de {numero1} + {numero2} es igual a {suma}")





# 7. Operaciones normales                   #Autor script: A.D
# En python también podemos usar operaciones para nuestros programas

# Sumas
suma = 10 + 10

# Restas
resta = 20 - 10

# Multiplicación
multiplicacion = 10 * 10

# División
division = 100 / 10

# División al piso
division_piso = 1000 // 100

# Elevado
elevado = 2 ** 3  # 2 elevado a la 3

# Raíz cuadrada
raiz = 1000 ** 0.5

# División_resto
resto = 10 % 3

print(f"La suma es {suma}")
print(f"La resta es {resta}")
print(f"La multiplicación es {multiplicacion}")
print(f"La división es {division}")
print(f"La división al piso es {division_piso}")
print(f"El elevado es {elevado}")
print(f"La raíz cuadrada es {raiz}")
print(f"El resto de la división es {resto}")






# 8. Round                    #Autor script: A.D
# Round es un método que se utiliza para redondear, simple

mi_float = 19.999999234923492934923492394923
tipo = str(type(mi_float))
print("Mi float sin redondear es de tipo " + tipo)

# Vamos a usar round
mi_float = str(round(mi_float, 2))  # Redondeado a 2 decimales
print("Resultado del redondeo: " + mi_float)


tipo = str(type(mi_float))
print("Mi float ha sido redondeado y ahora es de tipo " + tipo)

mi_float = 10.5
roundd = str(round(mi_float))
print(f"{mi_float} es ahora: {roundd}")






# 9. Index    
# Index es un metodo para sacar el indice de una cadena de texto           #Autor script: A.D

mi_string = "hola buenas tardes"
mi_string_index = mi_string.index("h")
print("La letra h se encuentra en el índice: ")
print(mi_string_index)





# 10. Métodos que se usan con string             Autor script: A.D
#Estos son algunos metodos que trae strings en python, mas adelante veremos una libreria llamada strings           
mi_string = "Hola buenas tardes"

print("Usando capitalize: ")
capitalizar = mi_string.capitalize()
print(capitalizar)

print("Usando upper")
upperr = mi_string.upper()
print(upperr)

print("Usando split")
spliteo = mi_string.split("e")
print(spliteo)

print("Usando join")
mi_string2 = "asfdadsf"
join = "".join([mi_string, mi_string2])
print(join)

#Join necesita usar listas o tuplas para poder trabajar, no puede haber un join asi:
#join = "".join(mi_string,mi_string2)          no podria ser eso posible a menos que hagamos esto:
#strings = [mi_string,mi_string2]  y luego:
#join = "".join(strings)


print("Usando find")
find = mi_string2.find("f")
print(find)

print("Usando replace")
replace = mi_string2.replace("f", "z")
print(replace)






# 11. Propiedades de los Strings                     #Autor script: A.D
# Ya sabemos que los strings son cadenas de texto y son inmutables

mi_string = "Hola"

# mi_string[0] = "a"     ESTO NO SE PUEDE HACER NO PODEMOS MODIFICAR EL CONTENIDO DE UN STRING

# PERO SI QUE PODEMOS CAMBIAR SU CONTENIDO
mi_string = "Nuevo contenido del string"

# No podemos por ejemplo multiplicar un string por un número

# mi_string = mi_string * 10 - 2      ERROR

# Podemos obtener el número de caracteres que tiene un string usando len
uso_len = len(mi_string)
print(uso_len)

# Podemos ver si una letra se encuentra en nuestro string y obtener un boolean de respuesta
print("o" in mi_string)






# 12. Booleanos                                 #Autor script: A.D
# Los booleanos nos devuelven dos tipos de respuesta ante una condición
# Nos pueden devolver true
# o false

mi_boolean1 = True
mi_boolean2 = False

print(mi_boolean1 == mi_boolean2)

resultado = 1000 * 123123123
resultado2 = 234234 * 234234234 / 23423

print(resultado == resultado2)  # resultado de false





# 13. LISTAS                                     #Autor script: A.D
# Las listas son un conjunto de elementos organizados
# Pueden contener dentro de ellas cualquier tipo de valor
# Las listas se usan con []

lista_integers = [1, 2, 3, 4, 5, 6, 23, 234, 45234]
print("La lista de integers: ")
print(lista_integers)

print("Añadir")
lista_integers.append(10)
print(lista_integers)

print("Eliminar integer")
eliminar = lista_integers.pop(1)
print(lista_integers)

print("Ordenar integers")
lista_integers.sort()
print(lista_integers)

lista_strings = ["Pablo", "Raul", "Carmen", "Alex"]
print("La lista de strings:")
print(lista_strings)

print("Añadir una nueva persona")
lista_strings.append("Nueva persona")
print(lista_strings)

print("Eliminar una persona")
eliminar = lista_strings.pop(3)
print(lista_strings)

print("Ordenar la lista en orden alfabético")
lista_strings.sort()
print(lista_strings)

# Hay que destacar que en python y en muchos otros lenguajes no solo hay colecciones
# como las listas, también están los diccionarios, los sets, las tuplas... etc




# 14. Diccionarios                          #Autor script: A.D
# Los diccionarios en python son un conjunto de elementos divididos en clave y valor
# Básicamente una palabra con un significado igual que en un diccionario
# Se escriben con {}

mi_diccionario = {"clave": "valor", "clave2": "valor2", "clave3": "valor3"}
print("El diccionario es:")
print(mi_diccionario)

# Podemos imprimir solo las palabras clave del diccionario
keyss = mi_diccionario.keys()
print(keyss)

# Al igual que podemos imprimir los valores del diccionario
valores = mi_diccionario.values()
print(valores)

# Pueden haber diccionarios dentro de otros diccionarios
diccionario_en_diccionario = {"clave1": {"valor1": "valor2"}}
print("Diccionario en otro diccionario:")
print(diccionario_en_diccionario)
print(diccionario_en_diccionario.keys())
print(diccionario_en_diccionario.values())





# 15. TUPLAS                            #Autor script: A.D
# Las tuplas son un conjunto de elementos también, son parecidos a las listas
# de strings, son inmutables y su contenido no se puede modificar
# Las tuplas se escriben con ()
mi_tupla = (1, 232, 23, 23, 23)

# Las tuplas también tienen métodos igual que otras colecciones de elementos
print(mi_tupla.count(23))

print(mi_tupla[0])





# 16. LOS SETS                            #Autor script: A.D
# Los sets son un conjunto desorganizado de elementos únicos
# Se usan {} para los sets

mi_set = {1, 2, 3, 4, 5, 6}

mi_set.add(7)
print(mi_set)

mi_set.remove(4)
print(mi_set)

# Los sets tienen el método de discard
mi_set.discard(100000)
# En caso de que el valor no exista no va a dar error

# Esto daría ERROR:
# print(mi_set[1])
# NO se pueden modificar los elementos de los sets ya que están desorganizados
# y son únicos

# Pero si se pueden usar métodos como remove o así
mi_set.remove(6)
print(mi_set)




# 17. Operadores de comparación                     #Autor script: A.D
# Los operadores de comparación nos devuelven un boolean como resultado
# Son estos:

print("==")
operador_comparacion1 = 2 == 2
print(operador_comparacion1)

print("!=")
operador_comparacion2 = 2 != 2
print(operador_comparacion2)

print("<")
operador_comparacion3 = 3 < 4
print(operador_comparacion3)

print(">")
operador_comparacion4 = 4 > 3
print(operador_comparacion4)

print(">=")
operador_comparacion5 = 3 >= 3
print(operador_comparacion5)

print("<=")
operador_comparacion6 = 3 <= 9
print(operador_comparacion6)




# 18. Operadores lógicos                             #Autor script: A.D
# Los operadores lógicos se utilizan para ejecutar algo si se cumple una condición
# Son OR, AND y NOT

resultado1 = 1 == 1
resultado2 = 1 == 2

print(resultado1)
print(type(resultado1))

print(resultado2)
print(type(resultado2))

print(resultado1 == resultado1 and resultado2 == resultado2)
print(resultado1 == resultado1 or resultado2 == resultado2)
print(not resultado1 == resultado2)


# Más complejo
print(resultado1 == resultado1 and resultado1 == 1 or resultado2 == resultado2)
print(resultado1 == 23423 or resultado1 == 3242342342 or resultado1 == 324234 or resultado1 == resultado1)
print(resultado1 == 23423 or resultado1 == 3242342342 or resultado1 == 324234 or resultado1 == resultado1 and resultado2 == resultado2 and resultado2 == 243234234234)
print(not resultado1 == resultado2 or not resultado1 == resultado1)




# 19. Controles de flujo                              #Autor script: A.D
# Con los controles de flujo creamos estructuras de código que se ejecutarán 
# si se cumplen ciertas condiciones
# Los controles de flujo son if, else y elif

#If es para ver si una condicion se cumple o no
#Elif es por si el if no se cumple pues se intenta elif
#Else es por si ningun if o elif se cumple

numero1 = 1
numero2 = 2

if numero1 == numero2:
    print("Número1 es igual a número2")
else:
    print("Parece que número1 y número2 son diferentes")

string1 = "hola"
string2 = "hola"

if string1 == string2:
    print("String1 y string2 son iguales")
elif string1 == string2:
    print("Te estoy diciendo otra vez que string1 y string2 son iguales")
elif string2 == string1:
    print("Y otra vez... xD")
else:
    print("Los strings no son iguales")

operacion1 = 24234234 * 234234 - 234234234 / 23423424
operacion2 = 1 + 1

if not operacion1 == operacion2:
    print("La operación1 y la operación2 no son iguales")
else:
    print("Las operaciones obviamente sí que son iguales")





# 20. Loop for                             #Autor script: A.D
# El loop for se utiliza para recorrer una lista de elementos o una colección
# y poder hacer cualquier cosa con estos elementos
# Dentro de los bucles podemos usar controles de flujo como if, else o elif

lista_numeros = [1, 2, 3, 4, 5]

for numero in lista_numeros:
    print(numero)

for numero in lista_numeros:
    numero = numero + 1
    print("Ahora el número sumado más uno es igual a: ")
    print(numero)

for numero in lista_numeros:
    if numero == 2:
        print("Parece que este elemento de la lista es igual a 2")
    else:
        print("Este elemento no es igual a 2")

for numero in lista_numeros:
    if numero == 2 or numero == 1 or numero == 3:
        print("Parece que este elemento de la lista es igual a 1, 2 o 3")
    else:
        print("Este elemento no es ni 1, ni 2, ni 3")

# 21. Loop while                              #Autor script: A.D
# Los bucles while se utilizan para ejecutar una acción hasta que una condición
# se cumpla
# Hay que tener cuidado con los bucles while porque si los hacemos mal pueden ejecutar una condición
# infinitamente en el código sin acabar
#Break es para detener un bucle while

numero1 = 1000
numero2 = 2000

while numero1 < numero2:
    numero1 = numero1 + 100
    print(numero1)

numero1 = 0
numero2 = 30

while numero1 < numero2:
    numero1 = numero1 + 10
    if numero1 == 30:
        print("Parece que el elemento se ha ido sumando y ha llegado hasta 30")
    else:
        print("Parece que el elemento sumado todavía no ha llegado hasta 30")


numero_nuevo = 0
while True:
    numero_nuevo = numero_nuevo + 2
    if numero_nuevo == 30:
        print("Ya ha llegado hasta 30")
        break





# 22. Range                         #Autor script: A.D
# Range es una palabra reservada en Python y dentro de sus parámetros podemos indicar la longitud

for x in range(10):
    print("Elemento:")
    print(x)
    print("\n")


lista = list(range(1, 30))
print(lista)
for elemento in lista:
    print(elemento)





# 23. Enumerate                       #Autor script: A.D
# Enumerate es una palabra reservada 
# para enumerar automáticamente los elementos
# de una lista que le pasemos

lista = ["a", "b", "c"]

lista_enumerada = list(enumerate(lista))
print(lista_enumerada)

for elemento in lista_enumerada:
    print(elemento)





# 24. Zip                           #Autor del script: A.D
# Zip es una palabra reservada para unir dos listas

nombres = ["Alex", "Raul", "Marta", "Paquita"]
print("Los nombres")
print(nombres)
edades = [120, 0.1, 0.1, 0.1]
print("Edades respectivas:")
print(edades)

uso_zip = list(zip(nombres, edades))
print("Zipeando las listas:")
print(uso_zip)





# 25. Min y Max                               #Autor del script: A.D
# Son palabras reservadas de Python para obtener
# el máximo o el mínimo de una lista

# Se puede hacer esto para listas de números
lista_numeros = [1, 2, 3, 4, 5]
print("La lista de números:")
print(lista_numeros)

min_lista_numeros = min(lista_numeros)
print("Mínimo de la lista:")
print(min_lista_numeros)

max_lista_numeros = max(lista_numeros)
print("El máximo de la lista de números es:")
print(max_lista_numeros)



# Pero también se puede hacer para strings
# Se clasificará por menor o mayor según el orden de la primera letra de cada palabra
lista_strings = ["Arbol", "Barcelona", "Carmen", "David", "ESPAÑA"]
print("La lista de strings:")
print(lista_strings)

print("El mínimo de la lista de strings:")
minimo_lista_strings = min(lista_strings)
print(minimo_lista_strings)

print("El máximo de la lista de strings:")
maximo_lista_strings = max(lista_strings)
print(maximo_lista_strings)





# 26. Random                            #Autor del script: A.D
# Random es una librería para aleatorizar elementos automáticamente
# Trae métodos como randint o choice
# IMPORTANTE: esta librería no está en Python por defecto así que vamos 
# a tener que importarla arriba del código que se hace por convencion pero tambien 
#se puede hacer en mitad del codigo


from random import randint as r, choice as c

numero_random = r(1, 50)
numero_random2 = r(1, 100)

print("El primer número random es " + str(numero_random))
print("El segundo número random es " + str(numero_random2))

lista_numeros_bingopremio = [112312, 12312312, 3453434, 123123, 567, 23423423, 23423, 423423, 4234]
print("Los números de los posibles ganadores del sorteo son:")
print(lista_numeros_bingopremio)
print("\n")
elegir_choice = c(lista_numeros_bingopremio)
print("El número elegido ganador del premio es " + str(elegir_choice))





# 27. Match                              #Autor del script: A.D
# El match en Python es como el switch de Java
# Se usa para evaluar una variable con distintos casos
# Si se cumplen esas condiciones en los casos
# Se ejecuta un código deseado por el programador

lista_colores = ["azul", "rojo", "verde"]

for color in lista_colores:
    match color:
        case "rojo":
            print("Parece que está el color rojo en la lista de colores")


operacion = 10 + 10 - 6  # (14)
match operacion:
    case 20:
        print("El resultado de la operación es igual a 20")
    case 30:
        print("El resultado es igual a 30")
    case 14:
        print("El resultado es igual a 14")





# 28. Funciones                 #Autor del script: A.D
# Las funciones son métodos propios que nosotros mismos creamos
# y que podemos usar con nuestras variables como si fueran métodos normales

def saludo():
    print("Esto es lo que hace la función de saludo, pues saludar carajo xD")

saludo()

def sumar():
    num1 = 4
    num2 = 2
    resultado = num1 + num2
    print(f"{num1} + {num2} es igual a {resultado}")
sumar()

def restar(num1, num2):
    resultado_resta = num1 - num2
    print(resultado_resta)
restar(10, 5)    





# 29. Return
# Return se usa en las funciones para devolver un valor aunque 
# no sea impreso

def restar(num1, num2):
    resultado_resta = num1 - num2
    return resultado_resta

resultado = restar(10, 5)
print(resultado)





# 30. Interacción entre funciones

# 1. Crear palitos
palitos = ["-", "--", "---", "----"]

# 2. Mezclar palitos
from random import shuffle

def mezclar_palitos(palitos):
    shuffle(palitos)
    return palitos

# 3. Pedirle un intento al jugador
def pedir_intento():
    intentos = 3
    while intentos > 0:
        intento_usuario = int(input("Elige un palito: [1], [2], [3], [4]")) - 1
        if intento_usuario == 1:  # Suponiendo que el palito correcto es el segundo
            print("¡Acertaste!")
            break
        else:
            print("Vuelve a intentarlo")
            intentos -= 1
    if intentos == 0:
        print("Se te han acabado los intentos")


# Función principal
def juego():
    palitos_mezclados = mezclar_palitos(palitos)
    print(f"La lista de palitos es {palitos_mezclados}")
    pedir_intento()

# Ejecutar el juego
juego()





# 31. Args                   #Autor script: A.D
# Los args se ponen en los parámetros por ejemplo de una función
# Indican que se puede poner todos los parámetros que se desee
# sin ningún tipo de límite


def sumar(*args):
    total = sum(args)
    return total

resultado = sumar(1, 123, 123, 123, 123, 123, 123, 123, 123, 12, 312, 31)
print(resultado)

def sumar_y_print(*args):
    for arg in args:
        print(arg + arg)

sumar_y_print(1, 2, 3, 4, 5)





# 32. CLASES                     #Autor script: A.D
# Las clases en Python son plantillas para objetos donde podemos meter métodos y 
# atributos a ese objeto

# Creamos la clase
class Animal():
    # Definimos los atributos
    def __init__(self, color, años):
        self.color = color
        self.años = años
        
    # Definimos el método de volar
    def volar(self):
        print("Está volando")

    def saludar(self):
        print("No te puede saludar, es un maldito animal")

# Creamos una instancia de Animal llamada pájaro y le pasamos como parámetros
# los atributos que habíamos definido en la clase
pajaro = Animal("azul", 10)

# Creamos un método a la instancia que ya había sido creado en la clase
volar_pajaro = pajaro.volar()
saludar_pajaro = pajaro.saludar()

# Imprimimos los métodos de la instancia pájaro de animal
print(volar_pajaro) 
print(saludar_pajaro)

# Imprimimos los atributos de la instancia
print(pajaro.color)
print(pajaro.años)





# 33. HERENCIA                #Autor script: A.D
# La herencia consiste en que una clase hereda todos los métodos y los atributos de su clase padre
# Esto se hace mediante paréntesis

class Persona():
    def __init__(self, edad):
        self.edad = edad

    def saludar(self):
        print("Hola")

class Paco(Persona):
    pass

instancia_paco = Paco(16)
print(instancia_paco.edad)
instancia_paco.saludar()




# 34. POLIMORFISMO
#El polimorfismo consiste en cuando en nuestro codigo se usan por ejemplo metodos de diferentes clases
#en una misma lista, para que lo entendais es como mezclar partes del codigo en nuestro script

class Vaca():    
    def ruido(self):
        print("Hace muuu")

class Oveja():  
    def ruido(self):
        print("Hace beeee")

instancia_vaca = Vaca()
instancia_oveja = Oveja()

lista_animales = [instancia_oveja, instancia_vaca]
for animal in lista_animales:
    animal.ruido()





# 35. MÉTODOS ESPECIALES                 #Autor script: A.D
# Los métodos especiales en Python son aquellos que ya vienen por defecto
# Vienen con __ __
# Por ejemplo __init__ permite establecer los atributos a una clase
class No_Se():
    def __str__(self):
        return "Esto lo estoy escribiendo sin paréntesis gracias al método especial de __str__"
    
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def __len__(self):
        return len(self.nombre)

objeto = No_Se("Python", 30)
print(objeto)
print(len(objeto))




# 36. CONVENCIONES EN PYTHON
# Las convenciones de Python son aquellas "normas" por así decirlo,
# son un estándar de normas de cómo se debe de usar el código Python. 
# Estas son algunas:
"""
Usa 4 espacios por nivel de indentación.
Las líneas deben tener un máximo de 79 caracteres.
Usa una línea en blanco para separar funciones y clases, y dos líneas para separar secciones grandes de código.
Nombra las funciones, variables y atributos de instancia con letras minúsculas y palabras separadas por guiones bajos.
Nombra las clases y excepciones usando EstiloCamelCase.
Nombra las constantes usando letras mayúsculas y guiones bajos.
Usa una importación por línea.
Ordena las importaciones en grupos: primero las importaciones estándar, luego las de terceros, y finalmente las importaciones locales.
Coloca la sentencia import en la parte superior del archivo.
Usa espacios alrededor de operadores y después de comas, pero no directamente dentro de paréntesis, corchetes o llaves.
Coloca el docstring de una función o método justo después de la definición.
Utiliza comentarios para explicar el código, pero no en exceso.
Usa cadenas de formato en lugar de la concatenación de cadenas para crear mensajes.
Evita el uso de espacios en blanco finales.
Usa el manejo de excepciones para capturar errores en lugar de usar condiciones.
Sigue la convención de nombres __nombre__ para métodos y atributos que no deben ser accesibles desde fuera de la clase.
"""




# 37. Instalar paquetes                     #Autor script: A.D
# Un paquete es una colección de módulos organizados en un código que implementan
# nuevas funciones a Python para que las usemos
# Para instalar paquetes nos tenemos que ir al CMD (La línea de comandos)
# y escribir `pip install "nombre del paquete"`
# Por ejemplo si yo quiero instalar random escribo en CMD:
# pip install random 




# 38. EXCEPCIONES                    #Autor script: A.D
# Las excepciones en programación son una manera de manejar un error que sucede en el programa
# capturarlo y así poder ejecutar otra cosa en caso de que haya un error
# Las excepciones unchecked son las que ocurren sin que hagamos un try y except
# Y las checked son las que controlamos nosotros

numero1 = 10
numero2 = 0

# Esto de aquí son checked
try:
    numero2 / numero1
except ZeroDivisionError:
    print("No se puede dividir 10 entre 0")

try:
    numero2 / numero1
except Exception as e:
    print(f"Error: {e}")

# Si no lo hubiéramos puesto el código habría lanzado la excepción automáticamente





# 39. DECORADORES                  #Autor script: A.D
# Los decoradores son funciones que aceptan como parámetro otras funciones

def mayuscula(texto):
    print(texto.upper())
mi_funcion = mayuscula
mayuscula("esto va a ser uppeado")

def una_funcion(funcion):
    return funcion
una_funcion(mayuscula)

def decorador(funcion):
    def funcion_decorada():
        print("Antes")
        funcion()
        print("Después")
    return funcion_decorada

@decorador
def saludar():
    print("Hola")
saludar()






# 40. GENERADORES                         #Autor script: A.D
# Los generadores en Python son funciones que nos van devolviendo un resultado poco a poco
# Para que sea un generador tenemos que utilizar yield

def funcion_generadora():
    yield "siguiente"
    yield "siguiente"
    yield "siguiente"
    yield "siguiente"

generador = funcion_generadora()

print(next(generador))
print(next(generador))

print("Ejecutando otra tarea de código mientras el generador está pendiente...")
print(2 + 2)

print(next(generador))
print(next(generador))






# 41. DATETIME DATE                            #Autor script: A.D
# Datetime DATE es una librería que nos permite crear y manipular fechas con días

import datetime

fecha = datetime.date(2007, 8, 1)

print("La fecha de mi nacimiento es:")
print(fecha)

fecha2 = datetime.date.today()
print("La fecha actual es: ")
print(fecha2)

 



# 42. DATETIME TIME                     #Autor script: A.D
# Lo mismo que datetime date pero para horas específicas

hora_actual = datetime.time(12, 49, 58)
print("La hora actual es:")
print(hora_actual)

hora_actual2 = datetime.datetime.now().time()
print("La hora actual con datetime.now() es:")
print(hora_actual2)




# 43. DATETIME DATETIME                   #Autor script: A.D
# Es un conjunto de datetime date y datetime time

fecha_datetime = datetime.datetime(2007, 8, 1, 3, 35, 2)

print("Con datetime hacemos la fecha completa:")
print(fecha_datetime)




 
#44.MANIPULAR EL TIEMPO CON TIME           #Autor script: A.D

inicio = time.time()

for num in range(1, 5):
    print(num)

final = time.time()

tiempo_transcurrido = final - inicio
print("Tiempo transcurrido:", tiempo_transcurrido)






import math
import re
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
from cryptography.fernet import Fernet
import socket







#45.MATH                    #Autor script: A.D
import math  # Necesitas importar la librería math antes de utilizarla

# Math es una librería que nos permite hacer operaciones de manera más fácil
# que hacerlo manualmente
numero1 = 234234.234234

factorial_result = math.factorial(int(numero1))
print("Factorial:", factorial_result)

floor_result = math.floor(numero1)
print("Floor:", floor_result)

ceil_result = math.ceil(numero1)
print("Ceil:", ceil_result)

# Nota: La siguiente operación de potencia puede no ser práctica para números muy grandes
# power_result = math.pow(numero1, 324)
# print("Power:", power_result)





# 46. EXPRESIONES REGULARES                     #Autor script: A.D
# Son un módulo de Python que nos permite buscar patrones de texto en un texto
# hacemos un import re

Texto = "Python es un buen lenguaje de programacion"
palabra_a_buscar = "programacion"

busqueda = re.search(palabra_a_buscar, Texto)
print(busqueda)






# 47. EXPRESIONES LAMBDA                     #Autor script: A.D
# Las expresiones lambda son una manera de crear una función sin usar def 
# y crear una expresión simple útil y bastante legible

print("Lambda suma")
suma = lambda x, y: x + y
resultado_suma = suma(10, 10)
print(resultado_suma)

print("Lambda multiplicación")
multiplicacion = lambda x, y, z: x * y * z
resultado_multiplicacion = multiplicacion(5, 10, 8)
print(resultado_multiplicacion)

print("Lambda resta")
resta = lambda x, y: x - y
resultado_resta = resta(10, 5)
print(resultado_resta)

print("Lambda compleja")
expresion_lambda_compleja = lambda a, b, c, d, e: a * b * c - d + e * c / 2
resultado_lambda_compleja = expresion_lambda_compleja(234, 3534, 123, 345, 123)
print(resultado_lambda_compleja)

print("Lambda con strings")
lambda_strings = lambda string1, string2: string1 + string2
resultado_lambda_strings = lambda_strings("ho", "la")
print(resultado_lambda_strings)






# 48. FUNCIONES RECURSIVAS                 #Autor script: A.D
# Las funciones recursivas son aquellas que se llaman a sí mismas

def sumar(n):
    return 1 if n == 1 else n + sumar(n - 1)

resultado_suma = sumar(5)
print(resultado_suma)





# 49. ENUMERATE                   #Autor script: A.D

lista = ["a", "b", "c"]
lista_enumerada = list(enumerate(lista))
for enumerado in lista_enumerada:
    print(enumerado)

lista2 = ["valor1", "valor2", "valor3", "valor4"]
lista_enumerada2 = list(enumerate(lista2))
for enumerado in lista_enumerada2:
    print(enumerado)






# 50. PANDAS                   
# PANDAS es una librería para analizar datos y hacer con ellos como tablas de Excel en unos DataFrames
# Tenemos que hacer un import de ella

# dataframes = pd.read_csv("archivo.csv")
# print(dataframes)





# 51. NUMPY                    #Autor script: A.D
# Numpy es una librería para crear arrays de manera sencilla y para realizar operaciones con ella

# Así creamos un array
array = [1, 2, 3, 4, 5]
lista = np.array(array)
print(lista)

# Con arrange(6) creamos un array hasta 6
array_numeros = np.arange(6)
print(array_numeros)






# 52. MATPLOTLIB                  #Autor script: A.D
# Matplotlib es una librería para crear gráficos a partir de arrays, por ejemplo
# Personalmente me gusta más matplotlib que numpy o pandas
# Tenemos que hacer el import

lista1 = [1, 2, 3, 4, 5]
lista2 = [2, 4, 6, 8, 10]

plt.scatter(lista1, lista2)
plt.show()





# 53. CRYPTOGRAPHY                 #Autor script: A.D
# Es una biblioteca para generar contraseñas

contraseña = Fernet.generate_key()
print("La contraseña generada es " + contraseña.decode())





# 54. SOCKET                     #Autor script: A.D
# Socket es una librería para establecer conexiones entre dispositivos, ordenadores, servidores... etc

# mi_socket = socket.socket()
# mi_socket.connect(("localhost", 8080))
# mensaje_server = mi_socket.send(b"Hola servidor del puerto 8080")
# print(mensaje_server)





# 55. Capitalize                #Autor script: A.D
# Capitalize es un método que viene por defecto en Python
# Para imprimir la primera palabra de una cadena de texto en mayúscula

texto = "hola"
texto_capitalize = texto.capitalize()
print(texto_capitalize)






# 56. Upper                     #Autor script: A.D
# Upper es un método para transformar una cadena de texto minúscula en mayúscula

cadena_texto = "cadena de texto"
cadena_texto_upper = cadena_texto.upper()
print("La cadena de texto pasada a mayúscula es: ")
print(cadena_texto_upper)





import os
import random
import statistics

# 57. ISNUMERIC          #Autor script: A.D
# Es un método que se aplica a variables y devuelve como resultado un boolean
# True si es numérico y False si no es numérico, como por ejemplo, en el caso de un string.

cadena_NO_numerica = "Esto obviamente no es numerico y va a dar False"
es_numerico = cadena_NO_numerica.isnumeric()
print(f"El dicho de que esta cadena ({cadena_NO_numerica}) es numerica es: {es_numerico}")

# ESTO VA A DAR ERROR, PORQUE 'int' object has no attribute 'isnumeric'
# variable_numerica = 213123
# es_numerico = variable_numerica.isnumeric()
# print(f"El dicho de que esta variable ({variable_numerica}) es numerica es : {es_numerico}")






# 58. TUPLAS                 #Autor script: A.D
# Una tupla es un conjunto de elementos inmutables
#Disculpar si ya lo mencione antes, tengo mala memoria...

tupla = ("arbol", 123, "babaaaa")
tercer_elemento = tupla[2]
print(tercer_elemento)






# 59. ARITHMETIC ERROR           #Autor script: A.D
# Un... error aritmético?
try:
    10/0
except ArithmeticError:
    print("Ocurrió un error aritmético")






# 60. KEYBOARD INTERRUPT ERROR         #Autor script: A.D
# Es un error que se produce cuando el usuario le da al Ctrl C
try:
    numero1 = 10
    numero2 = 100000
    while numero1 < numero2:
        numero1 = numero1 + 1
        print(numero1)
except KeyboardInterrupt:
    print("El usuario ha pausado el programa")





# 61. EXCEPTION          #Autor script: A.D
# Es una excepción general normal
try:
    10/0
except Exception as e:
    print("Error de Exception")

variable = 7000 - 2000 * 2
try:
    variable/0
except Exception as e:
    print("Error de Exception")





# 62. TRY EXCEPT ELSE FINALLY            #Autor script: A.D
# Try es para intentar ejecutar un código
# Except es para manejar el error en caso de que surga y try no se ejecute
# Else es para ejecutar algo en caso de que try sí se cumpla
# Finally es para que el código se ejecute de todas maneras
try:
    10/5
except Exception:
    print("Esta división no es posible (MENTIRA)")
else:
    print("Este código se ejecuta en caso de que el try sea posible")
finally:
    print("Este código se ejecutará de todas maneras")



# Ejemplo 2
variable_string1 = "HOLA"
variable_string2 = "HOLA"

try:
    variable_string1 == variable_string2
except Exception:
    print("Esta división no es posible (MENTIRA)")
else:
    print("Este código se ejecuta en caso de que el try sea posible")
finally:
    print("Este código se ejecutará de todas maneras")




# 63. COMPARACIONES ENTRE ARRAYS               #Autor script: A.D
# Ejemplo 1
lista = [1, 2, 3, 4, 5, 6, 2]
lista2 = [1, 2, 3, 4, 5, 3, 2]
comparacion = lista < lista2
print(comparacion)


# Ejemplo 2
lista = [1, 2, 3, 4, 5, 6, 2]
lista2 = [1, 2, 3, 4, 5, 6, 2]
comparacion2 = lista <= lista2
print(comparacion2)

comparacion2_1 = lista == lista2
print(comparacion2_1)

comparacion2_2 = lista == lista2
print(comparacion2_2)

comparacion_2_3 = lista >= lista2
print(comparacion_2_3)





# 64. RANDOM CHOICE             #Autor script: A.D
# Choice es un método de random que sirve para escoger un elemento aleatorio
# de una lista que le indiquemos
lista = [1, 2, 3, 4, 4, 23, 423, 4, 23, 4, 23, 42, 34, 23, 4, 2, 34, 2]
print("La lista de premios es " + str(lista))
escoger = random.choice(lista)
print(escoger)


lista_nombres = ["Pablo", "Lucas", "Maria", "Lucia", "Raul"]
print("La lista de candidatos para el premio es: " + str(lista_nombres))
escoger_lista_nombres = random.choice(lista_nombres)
print("El alumno ganador es: " + escoger_lista_nombres)





# 65. RANDOM RANDAGE         #Autor script: A.D
# Es un método de random para elegir un elemento aleatoriamente
print("Eligiendo un numero aleatorio...")
variable_randage = random.randint(0, 10)
print("El ganador es " + str(variable_randage))





# 66. OS                 #Autor script: A.D
# Es para trabajar con el entorno actual del sistema
get_cwd = os.getcwd()
print("El directorio actual: ")
print(get_cwd)

proceso_actual = os.getpid()
print("El proceso actual: ")
print(proceso_actual)

entorno = os.getenv()
print("El entorno:")
print(entorno)






# 67. STATISTICS           #Autor script: A.D
# Es una librería para hacer operaciones con listas
print("USANDO STATISTICS")
lista = [1, 2, 3, 4, 5, 6, 7, 8]

print("Metodo mean:")
statistics_mean = statistics.mean(lista)
print("El elemento del medio de la lista es " + str(statistics_mean))

print("Metodo median:")
statistics_median = statistics.median(lista)
print("La media de la lista es " + str(statistics_median))

print("Metodo mode:")
statistics_mode = statistics.mode(lista)
print(str(statistics_mode))






import threading
import time
import multiprocessing
import sqlite3
import unittest


# 68. THREADING              #Autor script: A.D
# El threading multihilo consiste en ejecutar varios hilos de un mismo proceso a la vez.
# De esta manera nos ahorramos más tiempo distribuyendo todo mejor.
# La CPU se encarga de cada hilo a la vez.
# Tenemos que hacer el import threading.

# Creamos funciones
def saludar():
    print("Hola")

def despedirse():
    print("Adiós")

# Las almacenamos en un hilo
hilo1 = threading.Thread(target=saludar)
hilo2 = threading.Thread(target=despedirse)

# Las comenzamos
hilo1.start()
hilo2.start()

# Las terminamos
hilo1.join()
hilo2.join()





# 69. TIME                #Autor script: A.D
# Podemos usar esta librería para pausar la ejecución de un programa con el método sleep.
# Tenemos que hacer el import con import time.

print("LOADING---")
time.sleep(0.8)
print("LOADING------")
time.sleep(0.8)
print("LOADING---------")
time.sleep(0.8)
print("LOADING------------")
time.sleep(0.8)
print("------COMPLETE------")

lista = [1, 2, 3, 4, 5, 6]
for num in lista:
    print(num)
    time.sleep(0.8)




# 70. MULTIPROCESSING            #Autor script: A.D
# Lo mismo que con el multithreading pero ahora con multiprocessing.

def worker():
    print("Proceso:", multiprocessing.current_process().name)

if __name__ == "__main__":
    procesos = [multiprocessing.Process(target=worker) for _ in range(2)]
    [p.start() for p in procesos], [p.join() for p in procesos]





# 71. BASES DE DATOS               #Autor script: A.D
# Importamos sqlite3 o cx_Oracle (son las bases de datos).
# Podemos conectarnos a bases de datos de esta manera que suele ser la habitual:

# """
# connection = sqlite3.connect("Aqui tenemos que poner los datos de la base de datos")
# como puede ser el nombre de usuario, la contraseña, suelen ser 3 parámetros

# cursor = connection.cursor()

# cursor.execute("CREATE TABLE IF NOT EXIST ANIMALES(INT EDAD NOT NULL, NAME VARCHAR(300) NOT NULL)")
# cursor.execute("INSERT INTO ANIMALES (EDAD, NAME) VALUES(1,"PAJARO")")
# cursor.execute(SELECT * FROM ANIMALES)

# cursor.close()
# connection.close()
# """




# 72. UNITEST              #Autor script: A.D
# Es para ir testeando el código para ver errores.

# from mi_modulo import suma

class TestMiModulo(unittest.TestCase):

    def test_suma(self):
        self.assertEqual(suma(1, 2), 3)
        self.assertEqual(suma(-1, 1), 0)
        self.assertEqual(suma(-1, -1), -2)
        self.assertEqual(suma(0, 0), 0)

if __name__ == '__main__':
    unittest.main()





# 73. RAISE          #Autor script: A.D
# Es una palabra reservada de Python que sirve como si fuera un
# exception. Un ejemplo:

numero1 = 1
numero2 = 2

if numero1 == numero2:
    print("Son iguales")
else:
    raise Exception("Excepción por la cara xd")


def comprobar_igualdad(numero1, numero2):
    if numero1 == numero2:
        return "Son iguales"
    else:
        raise Exception("Excepción por la cara xd")




# 74. IDENTACIÓN            #Autor script: A.D
# Consiste en meter controles de flujo dentro de otros controles de flujo.

numero1 = 2
numero2 = 2
variable_a = "a"

if numero1 == numero2:
    print(f"{numero1} = {numero2}")
else:
    print("NO")
    if variable_a == variable_a:
        print("{variable1}")
    else:
        print("NO")
        if variable_a == variable_a:
            print("Variable a es igual a a")
        else:
            print("No es así")





# 75. Desempaquetado de secuencias          #Autor script: A.D
# Consiste en obtener los elementos de un array, por ejemplo, y almacenarlos en variables.

# Ejemplo 1
lista = [1, 2, 3, 4, 5]
a, b, c, d, e = lista
lista_elementos = lista
for elemento in lista_elementos:
    print(elemento)

# Ejemplo 2
lista2 = ["objeto1", "objeto2", "objeto3"]
a, b, c = lista2
lista3 = lista2
contador = 0

lista4 = []
for elemento in lista3:
    contador += 1
    nuevo_elemento = elemento + " elemento: " + str(contador)
    lista4.append(nuevo_elemento)

for elemento in lista4:
    print(elemento)





# 76. MACHINE LEARNING          #Autor script: A.D
# Consiste en hacer que nuestros programas aprendan por su cuenta,
# aprendan de los errores y nos hagan ellos solos la vida más fácil.

# Arriba del todo del código ponemos:
# from sklearn.linear_model import LinearRegression as ln

# Definición de las listas
lista_1 = [1, 2, 3, 4, 5]
lista_2 = [2, 4, 6, 8, 10]

import numpy as np
lista_1 = np.array(lista_1).reshape(-1, 1)
lista_2 = np.array(lista_2)

# Crear el modelo de regresión lineal
metodo = LinearRegression()

metodo.fit(lista_1, lista_2)

prediccion = metodo.predict([[6]])

# Imprimir la predicción
print(f"La predicción para 6 es: {prediccion[0]}")
print(f"La predicción para lista1 es: {lista_1[0][0]}")






# 77. GRAFOS            #Autor script: A.D
# Para que entendáis lo que es un grafo es como un mapa con distintos puntos que están conectados entre ellos.
# Cuando usamos grafos en programación son para ver todas las posibilidades que hay de los grafos con los demás grafos que hay.
# En el siguiente ejemplo se está viendo todas las posibles combinaciones entre Juan, Pablo y Carmen.

grafo = {
    "Juan": ["Juan, Pablo, Carmen"],
    "Pablo": ["Pablo", "Juan", "Carmen"],
    "Carmen": ["Juan, Pablo, Carmen"]
}

for persona, persona2 in grafo.items():
    print(f"{persona} conoce a {persona2}")





# 78. SLICES            #Autor script: A.D
# En Java, por ejemplo, para hacer slices usamos el método .split().
# En Python, para rebanar listas se hace con : y :: y poco más que yo sepa.

lista = [10, 20, 30, 40, 50]

# Aquí elige los elementos del 1 hasta el 4
sub_lista1 = lista[1:4]
print(sub_lista1)

# Aquí elige los elementos desde el segundo al quinto saltando de dos en dos
sub_lista2 = lista[1:4:2]
print(sub_lista2)

# Esto es para imprimir todos los elementos de la lista
sub_lista3 = lista[::]
print(sub_lista3)

# Esto imprime todos los elementos desde el primero hasta el final
sub_lista4 = lista[1::]
print(sub_lista4)

# Esto no me acuerdo sorry
sub_lista5 = lista[:4:]
print(sub_lista5)

# Esto ya lo sabemos de anterior código, imprime el primer y cuarto elemento
seleccion = [lista[0], lista[3]]
print(seleccion)





# 79. DEQUE               #Autor script: A.D
# Deque es una librería para manejar colecciones con elementos y poder operar con sus elementos de izquierda y derecha.

from collections import deque as dq

# Creamos un deque y le añadimos elementos con append()
d = dq()

d.append(1)
d.append(2)

# Esta es la parte importante de deque:
# Esto elimina el primer elemento de la izquierda
d.popleft()

# Esto añade al principio un 1
d.appendleft(1)

# Esto es para añadir un elemento al final del deque
d.append(3)

# Esto lo que hace es eliminar el elemento de la derecha
d.pop()




# 80. Crear listas con lógica          #Autor script: A.D
# Podemos crear una lista metiendo elementos si se cumple una condición.
# De esta forma estamos creando listas con elementos si cumplen algo de manera más directa.

lista_con_logica = [x for x in range(10) if x > 5]

for elemento_logico in lista_con_logica:
    x = elemento_logico + 10
    if x > 30:
        print("Un elemento mayor que 30: " + str(x))
    else:
        print("Un elemento menor que 30: " + str(x))





#81.Docstrings             #Autor script: A.D
#Los docstrings son cadenas de texto que pueden ser usados como comentarios
#o pueden ser usados en variables pero no se suelen hacer para cosas demasiado complejas
#como meterlas dentro de funciones, suelen ser principalmente para meterlo en variables
#como listas o usarlos como comentarios


def saludar(nombre):
    """
    Imprime el nombre pasado como argumento.
    """
    print(nombre)


saludar("Alex")


doc_string = ["""
Este texto esta siendo escrito dentro
          de un string
          """]

print(doc_string)





#82.INTERPRETE EN PYTHON             #Autor script: A.D
#Vale pues el intérprete de Python es 
#un programa específico para ejecutar código Python. 
#Yo personalmente no lo suelo usar demasiado pero es importante
#saber que esta ahi para usarlo, es como una terminal, aunque yo
#recomiendo ejecutar los programas con el boton normal de play. Un ejemplo de interprete:

"""
$ python
Python 3.9.7 (default, Oct 14 2021, 17:59:51)
[GCC 11.1.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> print("¡Hola, mundo!")
¡Hola, mundo!
>>> x = 5
>>> x * 2
10
"""





#83.Tipado dinamico                #Autor script: A.D
#Se que tendria que haber explicado esto antes pero bueno...

#Consiste en cambiar el tipo de una variable a otra en mitad del programa


#Integer:
variable_tipado_dinamico = 1
print("La variable de tipado dinamico es de tipo:" + type(variable_tipado_dinamico))


#String:
variable_tipado_dinamico = "Hola"
print("La variable de tipado dinamico es de tipo:" + type(variable_tipado_dinamico))


#Float:
variable_tipado_dinamico = 1.5
print("La variable de tipado dinamico es de tipo:" + type(variable_tipado_dinamico))


#Creo que long(no estoy seguro)
variable_tipado_dinamico = 1234234234
print("La variable de tipado dinamico es de tipo:" + type(variable_tipado_dinamico))




 
#84.CONTINUE                         #Autor script: A.D
#Continue sirve para en un bucle por ejemplo
#si se cumple una condicion que esta se omita
#Ejemplo:


lista_letras = ["a", "b", "c", "d", "e"]

mensaje = "La lista de letras es: " + ", ".join(lista_letras) + " y vamos a omitir la 'a' en el loop for"
print(mensaje)

for letra in lista_letras:
    if letra == "a":
        continue
    print(letra)

#En este codigo basicamente se omitira la a en el proceso de iterar cada elemento de la lista
#con un for y como es a y estamos usando continue no se imprimira





#85.ARGUMENTOS PREDETERMINADOS EN FUNCIONES          #Autor script: A.D

def saludar(mensaje = "Este mensaje esta en los parametros de la funcion saludar y va a ser impreso por el contenido de la funcion"):
    print(mensaje)

#Al llamar al metodo saludar imprimira lo que ya hemos metido en la funcion con el argumento predeterminado
saludar()

#Aqui le estamos metiendo un nuevo argumento
saludar("Nuevo argumento en los parentesis")





#86.MAP              #Autor script: A.D
#Map es un metodo que aplica una funcion especifica a una lista de elementos
#Se puede usar map con nuestros metodos propios o mismamente con una expresion lambda

#Ejemplo 1
lista_numeros_map = [1,2,3,4,5]

def mi_funcion(x):
    return x + 10

mapeado = list(map(mi_funcion,lista_numeros_map))


#Ejemplo 2
#Podemos usar map perfectamente para hacer casting de strings a integer
lista_numeros_map2 = ["13","26","33","44","52"]

mapear = map(int,lista_numeros_map2)

for numero in map:
    print(f"{numero} es de tipo {type(numero)}")



#Ejemplo 3
#Tambien podemos hacer casting de integers a strings
lista_numeros_map3 = [13,234,234,234,234,234]

mapeo3 = list(map(str,lista_numeros_map3))

print(mapeo3)


#Resumiendo: para usar map la forma normal seria crear una lista de elementos
#y por otro lado la funcion que queremos mapear a cada uno de esos elementos
#luego creamos una variable donde usamos map y le pasamos como parametros primero
#la funcion y luego la lista o lo que sea





#87.FILTER              #Autor script: A.D
#Es parecido a map, en vez de mapear funciones a listas lo que hace es filtrar
#elementos con condiciones, por eso se llama filter de filtrar me imagino...
#Se usa en buena parte con lambda


#Ejemplo 1
lista_numeros_filter = [1,2,3,4,5,6,7]

filtrar_filter_3 = filter(lambda x: x > 3, lista_numeros_filter)


#Ejemplo 2
lista_filter_pares = [123,213,222,21312,444,12312,13]

filtrar_filter_pares = filter(lambda x: x % 2==0, lista_filter_pares)

print(f"Los numeros pares son: {list(filtrar_filter_pares)}")






#88.WITH                 #Autor script: A.D
#With es una palabra reservada para ejecutar codigo a partir de recursos
#es una declaracion, seria como decirle al codigo algo asi:
#Oye con este archivo abierto, si el archivo esta abierto quiero que me ejecutes esto: blablabla


"""

with open("archivo.txt", "r") as archivo:
    contenido = archivo.read()
    print(contenido)

"""
#En ese ejemplo estamos diciendo: vale con el archivo abierto quiero que me generes un read
#y tambien que me imprimas el contenido





#89.METODO .FORMAT()             #Autor script: A.D
#El metodo format se utiliza como su nombre dice para formatear variables como strings etc
#En mi opinion es algo tedioso de usar y prefiero personalmente usar el print(f"")


#Ejemplo 1
variable1 = "variable1"

string1 = "string2"

print("La variable1 es {0} y el string1 es {1}".format(variable1,string1))



#Ejemplo 2
# Definir variables
nombre = "Juan"
edad = 30

# Usar .format() con índices numéricos
print("Mi nombre es {0} y tengo {1} años.".format(nombre, edad))






#90 __SLOTS__             #Autor script: A.D
#Los slots son una caracteristica que asignamos a los atributos de las clases y restringirlos
#para indicar que los objetos que instancian de esas clases solo tienen permitido
#usar esos atributos que se han creado con __slots__


class Animal:
    __slots__ = ["beber", "jugar"]

perro = Animal()
beber = perro.beber = "beber"
jugar = perro.jugar = "jugar"
print(beber)
print(jugar)


#dormir = perro.dormir = "dormir"      
#ESTO daria ERROR ya que con el slots hemos definido 
#los atributos unicamente posibles para usar






#91.PICKLES SERIALIZACION             #Autor script: A.D
#Es una clase para serializar
#Serializacion es el proceso de convertir datos a una secuencia de bytes
#La serializacion se utiliza para almacenar mejor un dato y poder pasarselo a otra computadora
#Hacemos el import de pickle: import pickle as pkl

import pickle as pkl

#Ejemplo 1
datos_pickle = {"clave1": "valor1", "clave2": "valor2"}

pickle_data = pkl.dumps(datos_pickle)

print(pickle_data)



#Ejemplo 2
datos_pickle2 = [1,2,3,4,5,6,7]

pickle_2 = pkl.dumps(datos_pickle2)

print(f"La serializacion de {datos_pickle2} su resultado es: {pickle_2}")






#92.GZIP COMPRESION DE ARCHIVOS                    #Autor script: A.D
#Lo he puesto entre comillas porque el codigo puede dar error
"""
import gzip

# Datos a comprimir
datos = b"Este es un texto de ejemplo que será comprimido con Gzip."

# Comprimir los datos
with gzip.open("datos_comprimidos.gz", "wb") as archivo_comprimido:
    archivo_comprimido.write(datos)

# Descomprimir los datos
with gzip.open("datos_comprimidos.gz", "rb") as archivo_comprimido:
    datos_descomprimidos = archivo_comprimido.read()

print("Datos descomprimidos:", datos_descomprimidos.decode())

"""




#93.SECRETS PARA CONTRASEÑA                #Autor script: A.D
#Es obvio que es para generar contraseñas
#Es como cryptography parecido
#Tenemos que hacer el import secrets


import secrets as secrets  #a

token = secrets.token_bytes(16)

print(f"El token generado es {token}")





#94.SMTPLIB es para mandar mensajes por mail        #Autor script: A.D
#Lo he puesto otra vez entre comillas porque me da que va a dar error
#disculpar, quedaros con que teneis que usar smtplib la libreria
"""
import smtplib
from email.mime.text import MIMEText
from email.mime.multipart import MIMEMultipart
from email.mime.text import MIMEText
from email.mime.multipart import MIMEMultipart

# Configuración del servidor SMTP
smtp_server = 'smtp.example.com'
smtp_port = 587
smtp_username = 'tu_correo@example.com'
smtp_password = 'tu_contraseña'

# Configuración del correo electrónico
from_email = 'tu_correo@example.com'
to_email = 'destinatario@example.com'
subject = '¡Hola!'
body = 'Este es un correo de prueba enviado desde Python.'

# Crear el mensaje
message = MIMEMultipart()
message['From'] = from_email
message['To'] = to_email
message['Subject'] = subject
message.attach(MIMEText(body, 'plain'))

# Conexión al servidor SMTP
server = smtplib.SMTP(smtp_server, smtp_port)
server.starttls()  # Iniciar una conexión TLS (si el servidor lo admite)
server.login(smtp_username, smtp_password)

# Enviar el correo electrónico
server.sendmail(from_email, to_email, message.as_string())

# Cerrar la conexión
server.quit()

print("Correo electrónico enviado con éxito.")
"""





#95.SUBPROCESS                #Autor script: A.D
#Es una libreria para ejecutar comandos en la linea de comandos de python
#mediante el codigo de este IDE
#import subprocess arriba por convencion

#Ejemplo 1

subprocess.run(["python", "-m", "venv", "mi_entorno"])

subprocess.run(["print", ])


#Ejemplo 2
files = subprocess.run(["ls"], capture_output=True, text=True).stdout
print(files)





#96.STRINGS (me refiero a strings la libreria)                 #Autor script: A.D
#Esta libreria permite realizar operaciones con strngs
#Tenemos que hacer el import

print("ASCI NORMAL con strings la libreria")
asci = string.ascii_letters()
print(asci)

print("Ascii lower")
ascii_lower = string.ascii_lowercase()
print(ascii_lower)


print("Ascii upper")
ascii_upper = string.ascii_uppercase
print(ascii_upper)


print("Ascii digitos")
digitos = string.digits()
print(digitos)


print("Ascii octdigits")
octdigits = string.octdigits()
print(octdigits)


print("Ascii hexdigits")
hexdigits = string.hexdigits()
print(hexdigits)





#97.NUMBERS            #Autor script: A.D
#Para hacer operaciones con numeros
#hacemos el import numbers

def es_numero_complejo(obj):
    return isinstance(obj, numbers.Complex)

# Ejemplo de uso
print(es_numero_complejo(3 + 4j))  # Salida: True
print(es_numero_complejo(5))       # Salida: False





#98.DIFERENCIAS ENTRE CASTING Y PARSING

#Puede que hayais escuchado alguna vez la palabra casting o parsing
#Solo quiero dejar claro la diferencia entre estas porque se parecen por el nombre 
#y se pueden llegar a confundir.
#Parsing: es el proceso de sacar un elemento de una cadena o de una lista
#Casting: es el proceso de convertir una variable de un tipo de dato a otro que queramos



#Parsing
texto = "Fecha: 2024-06-19"
fecha = texto.split(": ")[1]  
print(fecha)  


texto = "Python es genial"
palabras = texto.split()  # Parsing para obtener las palabras
print(palabras)  # Output: ['Python', 'es', 'genial']
#CUIDADO: no debeis de confundir extraer un elemento de una lista con parsing
#La diferencia principal que teneis que saber es que el parsing consiste en descomponer
#las palabras de la lista



# Ejemplo de parsing sin que useis el metodo split
texto = "Fecha: 2024-06-19"
fecha = texto[7:]  
print(fecha)  





#Casting
numero_integer = 10
numero_float = float(numero_integer)


numero_float = 10.0
numero_integer = int(numero_float)


boolean = True
#numero_float = float(boolean)           Esto NO SE PUEDE hacer


cadena = "Esto es una cadena de texto string"
#cadena_int = int(cadena)        NO SE PUEDE HACER



# Intentar convertir una lista o diccionario en un entero o flotante
lista = [1, 2, 3]
diccionario = {"a": 1, "b": 2}
# int(lista)  # Error: TypeError: int() argument must be a string, a bytes-like object or a number, not 'list'
# float(diccionario)  # Error: TypeError: float() argument must be a string or a number, not 'dict'





#99.GLOBAL
#Vale global es bastante curioso, sirve para cuando se crea una variable normal fuera de una funcion
#si nosotros usamos global dentro de una funcion y esa variable tiene el mismo nombre que la que esta
#fuera entonces estamos diciendo al codigo que son la misma variable, en caso de que no pusieramos global
#y las variables tuvieran el mismo nombre no tendrian ningun tipo de relacion.
#Voy a poner un ejemplo con global y otro sin global para que se note la diferencia


#Ejemplo SIN GLOBAL
contador_no_global = 0

def incrementar_contador():
    contador_no_global = contador_no_global + 1

incrementar_contador()
print(contador_no_global)  # Output: 0



#EJEMPLO CON GLOBAL
contador_global = 0

def incrementar_contador2():
    global contador_global
    contador_global = contador_global + 1

incrementar_contador2()
print(contador_global)  # Output: 1



#Supongo que ya estareis viendo la diferencia entre global y no global
#Resumidamente global es para llamar a variables externas y usarlas en funciones
#Y al no usar global no va a haber relacion de variables





#100.APARTADO ADICIONAL              #Autor del script: A.D
#Esto es para deciros que si quereis dominar el lenguaje practicarlo un poco todos los dias
#Hacer programas simples, ve famialiarizandote con la POO(Programacion orientada a objetos)
#Y no te conformes con saber mi script, python esta en constante desarrollo
#Espero que haya servido chaoo

"""

😈

😈

😈


💻💻💻💻💻💻💻💻💻💻
PPPPPPPPPPPPPPPPPPPPPPPP
💻💻💻💻💻💻💻💻💻💻
YYYYYYYYYYYYYYYYYYYYYYYY
💻💻💻💻💻💻💻💻💻💻
TTTTTTTTTTTTTTTTTTTTTTTT
💻💻💻💻💻💻💻💻💻💻
HHHHHHHHHHHHHHHHHHHHHHHH
💻💻💻💻💻💻💻💻💻💻
OOOOOOOOOOOOOOOOOOOOOOOO
💻💻💻💻💻💻💻💻💻💻
NNNNNNNNNNNNNNNNNNNNNNNN


😈

😈

😈

Podeis usar emoticonos en vuestro codigo con Windows + . pero recordar que deben de ser en cadenas

"""




