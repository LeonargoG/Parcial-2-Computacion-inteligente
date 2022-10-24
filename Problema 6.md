**EJERCICIO 6**

Realiza un dfd que almacene en un vector todos los numeros pares leidos hasta completar los espacios

[![6-TO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/pddH7dM5/6-TO-PROBLEMA-WHILE.jpg)](https://postimg.cc/MngNfqTz)

[![6-TO-PROBLEMA-FOR.jpg](https://i.postimg.cc/1tk1fcnD/6-TO-PROBLEMA-FOR.jpg)](https://postimg.cc/9RYnk9Bf)

[![6-TO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/br1cbDkW/6-TO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/0K5B1Nt0)

**Prueba de esritorio**

|Corrida|Numero ingresado|%2?|%2-->(c)=N y C=c+1|
|-|-|-|-|
|1|6|si|(0)-->6 and c=1|
|2|4|si|(1)-->4 and C=2|
|3|3|no||

**Ejemplo del array hasta ahora**

|6|
|-|
|4|

**Ciclo for**
```
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)

print(f"los numeros son {listanumeros}")

def pares(listanumeros):
    listanumeros = []


for n in listanumeros:
    if n % 2 == 0:
        print("Estos numeros son pares"+ "  " + str(n))
```
**Ciclo while**

```
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
decision = input("¿desea añadadir mas numeros?: ")

while decision == "s" or decision == "s":
    numerousuario = int(input("introdusca otro numero: "))
    listanumeros.append(numerousuario)
    decision = input("¿desea añadir otro numero?: ")


print(f"los numeros son {listanumeros}")
for n in listanumeros:
    if n % 2 == 0:
        print("Este numero de la lista es par" + str(n))
        


input("por favor, precione una tecla para salir.")
```
**Ciclo Do-While**

```
print("PARES")
numero_1 = int(input("Escriba un número entero: "))
numero_2 = int(input(f"Escriba un número entero mayor o igual que {numero_1}: "))

if numero_2 < numero_1:
        print(f"¡Le he pedido un número entero mayor o igual que {numero_1}!")
else:
        for i in range(numero_1, numero_2 + 1):
            if i % 2 == 0:
                print(f"El número {i} es par.")
```
