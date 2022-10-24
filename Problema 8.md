**EJERCICIO 8**

Crea un dfd que capture N numeros en el rango [li,ls] donde LI=limite inferior y LS=Limite superior para li<ls y ls>0, obtener:
  
  Cantidad de numeros pares y su promedio
  
  Cantidad de numeros impares y su promedio
  
  ¿Que promedio es mayor?
 

[![8while.jpg](https://i.postimg.cc/ZKtQGqzs/8while.jpg)](https://postimg.cc/Z0Hj34R6)

[![8for.jpg](https://i.postimg.cc/3x9b0C4z/8for.jpg)](https://postimg.cc/sMQJtWJJ)

[![8dowhile.jpg](https://i.postimg.cc/qqfmH1S6/8dowhile.jpg)](https://postimg.cc/LYTkz3Hm)
  
  **Prueba de escritorio**
  
|Corrida|N|N%2?|si-->Sp=Sp+N and Cp=Cp+1|No--->Si=Si+N and Ci=Ci+1|
|-|-|-|-|-|
|1|5|no|...|Si:5 and Ci:1|
  |2|6|si|sp:6 and cp:1|
  |3|7|no|...|si:12 and ci:2|
  |4|2|si|si:7 and CP:2|
  
  **Ciclo for**
  
  ```
  sp=0
cp=0
pp=0
si=0
ci=0
pi=0
li=-1
ls=-1
n=-1
num=-1

while(li<0):
    li = int(input("Limite inferior: "))
    
    if(li<0):
        print("Tiene que ser mayor a 0")
        
while(ls<li):
    ls = int(input("Limite superior: "))
    
    if(ls<li):
        print("Tiene que ser mayor que el limite inferior")
        
while(n<0):
    n = int(input("¿Cuantos numeros? "))
    
    if(n<0):
        print("Tiene que ser mayor a 0")
    
for i in range(n): 
    while(num<=li or num>=ls):
        num = int(input("Dame un numero de LI y LS: "))
        
        if(num<=li or num>=ls):
            print("Tiene que estar dentro del LI al LS")

    if(num%2==0):
        sp=sp+num
        cp=cp+1
    else:
        si=si+num
        ci=ci+1
        
    num=-1       
         
if(sp==0 or cp==0):
    pp=0
else:
    pp=sp/cp
    
if(si==0 or ci==0):
    pi=0
else:
    pi=si/ci
    
if(pp>pi):
    print("El PP es mayor que el PI")
else:
    print("El PI es mayor que el PP")
  ```
  **Ciclo while**
  
  ```
  print("Dame Límite inferior: ")
Li = int(input())
while Li<0:
    print("El límite inferior debe ser mayor a 0")
    print("Dame Límite inferior: ")
    Li = int(input())

print("Dame límite superior: ")
Ls = int(input())
while Ls<=Li:
    print("El límite superior no puede ser menor o igual al limite inferior")
    print("Dame límite superior: ")
    Ls = int(input())
  ```
  **Ciclo Do-while**
  
  ```
  pares = 0
impares = 0

lista=[]
for x in range(10):
    valor=int(input("Ingrese un valor entero: "))
    lista.append(valor)
print(lista)

for a in lista:
    if a % 2 == 0:
        pares = pares + a
    else:
        impares = impares + a
print("La suma de los números pares es: ",pares)
print("La suma de los números impares es: ",impares)

prom_pares = pares / a
prom_impares = impares / a

print("El promedio de los números pares es: ",prom_pares)
print("El promedio de los números impares es: ",prom_impares)

if prom_pares > prom_impares:
    print("El promedio de los pares es mayor que el promedio de los impares.")
else:
    print("El promedio de los números impares es mayor que el promedio de los pares.")
  ```
