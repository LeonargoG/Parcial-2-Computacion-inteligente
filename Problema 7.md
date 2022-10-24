**EJERCICIO 7**

Realiza un dfd que obtenga el promedio de las calificacion aprobadas y la cantidad de alumnos reprobados, la calificacion entre 0 y 10 y el maximo de alumnos es de 15

[![7-MO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/YCFvDbkm/7-MO-PROBLEMA-WHILE.jpg)](https://postimg.cc/mPbZt3Pb)

[![7-MO-PROBLEMA-FOR.jpg](https://i.postimg.cc/661T9Dpv/7-MO-PROBLEMA-FOR.jpg)](https://postimg.cc/0rD9nXmk)

[![7-MO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/WpKbRg5m/7-MO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/yWmzcg4W)

**Prueba de escritorio**

|corrida|contador|numero de vector|N|N>6-->C+1 and print en vector|
|-|-|-|-|-|
|1|1|0|5||
|2|1|0|8|C=C+1 and (0)=N|
|3|2|1|9|C=c+1 and (1)=N|

Ejemplo del array hast ahora

|9|
|-|
|8|

**Ciclo en for**

```dart
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
