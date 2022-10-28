### Ejercicio 10. 
CATURE 10 NUMEROS ENTEROS POSITIVOS, DIGA CUAL ES MAYOR Y CUAL ES MENOR.
#### 1.1 Analisis. 
CAPTURAR 10 NUMEROS ENTEROS POSITIVOS, DESPUES CALCULAR CUAL NUMERO ES MAYOR Y CUAL ES MENOR.


#### 1.2 DFD.
[![44.jpg](https://i.postimg.cc/htK5gzBt/44.jpg)](https://postimg.cc/ykrPyNxM)
#### 1.3 Prueba de escritorio 
|A[11] |i=1 |i<=10|N |A[i]|N>0|NUM[i]=N|i++|NUM|MAYOR|i |i<=10|MAYOR>NUM[i]|MAYOR=NUM[i]|i++|MAYOR|MENOR=MAYOR|i |i<=10|MENOR<NUM[i]|MENOR=NUM[i]|i++|MENOR|
|------|----|-----|--|----|---|--------|---|---|-----|--|-----|------------|------------|---|-----|-----------|--|-----|------------|------------|---|-----|
|0     |1   |1<=10|1 |1   |1>0|1       |2  |1  |0    |1 |1<=10|0>1         |1           |2  |     |10         |1 |1<=10|10<1        |1           |2  |     |
|1     |2   |2<=10|2 |2   |2>0|2       |3  |2  |1    |2 |2<=10|1>2         |2           |3  |     |           |2 |2<=10|1<2         |            |3  |     |
|2     |3   |3<=10|3 |3   |3>0|3       |4  |3  |2    |3 |3<=10|2>3         |3           |4  |     |           |3 |3<=10|1<3         |            |4  |     |     
|3     |4   |4<=10|4 |4   |4>0|4       |5  |4  |3    |4 |4<=10|3>4         |4           |5  |     |           |4 |4<=10|1<4         |            |5  |     |
|4     |5   |5<=10|5 |5   |5>0|5       |6  |5  |4    |5 |5<=10|4>5         |5           |6  |     |           |5 |5<=10|1<5         |            |6  |     |
|5     |6   |6<=10|6 |6   |6>0|6       |7  |6  |5    |6 |6<=10|5>6         |6           |7  |     |           |6 |6<=10|1<6         |            |7  |     |
|6     |7   |7<=10|7 |7   |7>0|7       |8  |7  |6    |7 |7<=10|6>7         |7           |8  |     |           |7 |7<=10|1<7         |            |8  |     |
|7     |8   |8<=10|8 |8   |8>0|8       |9  |8  |7    |8 |8<=10|7>8         |8           |9  |     |           |8 |8<=10|1<8         |            |9  |     |
|8     |9   |9<=10|9 |8   |9>0|9       |10 |9  |8    |9 |9<=10|8>9         |9           |10 |     |           |9 |9<=10|1<9         |            |10 |     |
|9     |10  |10<=10|10|9  |10>0|10     |   |10 |9    |10|10<=10|9>10       |10          |   |10   |           |10|10<=10|1<10       |            |   |1    | 


#### 1.4 Entradas
Ninguna

#### 1.5 Salidas.
NUM

MAYOR

MENOR

#### 1.6 Codigo.
```py
lista = [10]
cant = int(input("¿Cuantos numeros desea capturar?"))
i=1
while i <= cant:
    n = int(input(f"{i} Ingrese un numero: "))
    lista.append(n)
    i+=1
print("Numero mayor es ",max(lista))
print("Numero menor es ",min(lista))
```

### Ejercicio 11. 
OBTEN LA DISTANCIA MAYOR ENTRE 2 NUMEROS CONCECUTIVOS EN UNA LISTA DE 10 NUMEROS.
#### 1.1 Analisis.
Insertar 10 numeros, posteriormente calcular la distancia de 2 en 2 numeros y decir cual es la mayor distancia.


#### 1.2 DFD
![12](https://user-images.githubusercontent.com/113395327/197684202-afbcfb05-e77c-4657-97aa-c9c7c5377989.png)
#### 1.3 Prueba de escritorio 
|DIS[9],NUM[10]|i=1 |i<=9 |N |N>0|NUM[i]=N|i++|i  |i<9|DIS=NUM[i]-NUM[i+1]|DIS<0|D[i]=DIS|D[i]=DIS*-1|i++|
|--------------|----|-----|--|---|--------|---|---|---|-------------------|-----|--------|-----------|---|
|0             |1   |1<=9 |1 |1>0|1       |2  |1  |1<9|1                  |1<0  |        |           |2  |
|1             |2   |2<=9 |2 |2>0|2       |3  |2  |2<9|1                  |1<0  |||3| 
|2             |3   |3<=9 |3 |3>0|3       |4  |3  |3<9|1                  |1<0  |||4|
|3             |4   |4<=9 |4 |4>0|4       |5  |4  |4<9|1                  |1<0  |||5|
|4             |5   |5<=9 |5 |5>0|5       |6  |5  |5<9|1                  |1<0  |||6|
|5             |6   |6<=9 |6 |6>0|6       |7  |6  |6<9|1                  |1<0  |||7|
|6             |7   |7<=9 |7 |7>0|7       |8  |7  |7<9|1                  |1<0  |||8|
|7             |8   |8<=9 |8 |8>0|8       |9  |8  |8<9|1                  |1<0  |||9|
|8             |9   |9<=9 |9 |9>0|9       |   |9  |   |1                  |1<0  |1       |  
|9             |


|MAYOR|i |i<9|MAYOR>D[i]|MAYOR=D[i]|i++|MAYOR|
|-----|--|---|----------|----------|---|-----|
|O    |1 |1<9|0>1       |1|2|
|1    |2 |2<9|1<2       | 2 |3|
|2    |3 |3<9|2<3       | 3|4|
|3    |4 |4<9|3<4       |4|5|
|4    |5 |5<9|4<5       |5|6|
|5    |6 |6<9|5<6       |6|7|
|6    |7 |7<9|6<7       |7|8|
|7    |8 |8<9|7<8       |8|9|
|8    |  |   |          |||9|

#### 1.4 Entradas.
n.
#### 1.5 Salidas.
mayor=d[i].
#### 1.6 Codigo.
```dart
import 'dart:io';
import 'dart:core';
void main() {
  var Re = 0;
  var mayor = 0;
  stdout.write('Ingresa tus numeros \n');
  var lista = List.filled(10, 0);
  for (var i = 0; i <= 9; i++) {
    int Entrada = int.parse(stdin.readLineSync()!);
    lista[i] = Entrada;
  }
  var diferencias = List.filled(9, 0);
  for (var j = 0; j <= 8; j++) {
    diferencias[j] = (lista[j] - lista[j + 1]);
  }
  mayor = diferencias[0];
  for (var k = 0; k <= 8; k++) {
    if (mayor < diferencias[k]) {
      mayor = diferencias[k];
    } else {}
  }
  stdout.write("Tu lista es ");
  print(lista);
  stdout.write("y sus diferencias son ");
  print(diferencias);
  print('La diferencia mayor es ');
  print(mayor);
}
```

### Ejercicio 12. Almacene en un vector el resultado de una tabla (10 numeros)
#### 1.1 Analisis. 
Al tamaño del array sera de 10, validaremos el numero de la tabla, en una condición de termino.
#### 1.2 DFD
![13](https://user-images.githubusercontent.com/113395327/197684095-af2797a3-870a-44fe-a951-5756dbb6a704.png)
#### 1.3 Prueba de escritorio 
|n|n>0|i|i<=9|A[i]= n * i|i+1|A|
|-|-|-|-|-|-|-|
|5|5>0|0|0<=9|A[0]= 5 * 0|0+1|0|
| |   |1|1<=9|A[1]= 5 * 1|1+1|5|
| |   |2|2<=9|A[2]= 5 * 2|2+1|10|
| |   |3|3<=9|A[3]= 5 * 3|3+1|15|
| |   |4|4<=9|A[4]= 5 * 4|4+1|20|
| |   |5|5<=9|A[5]= 5 * 5|5+1|25|
| |   |6|6<=9|A[6]= 5 * 6|6+1|30|
| |   |7|7<=9|A[7]= 5 * 7|7+1|35|
| |   |8|8<=9|A[8]= 5 * 8|8+1|40|
| |   |9|9<=9|A[9]= 5 * 9|9+1|45|
#### 1.4 Entradas.
n.
#### 1.5 Salidas.
Mayor.
#### 1.6 Codigo.
```dart
import 'dart:io';
void main(List<String> args) {
  var array = [];
  int n = int.parse(stdin.readLineSync()!);
  for (var i = 0; i < 11; i++) {
    array.add(i);
    array[i] = n * i;
  }
  print('$array');
}
```

### Ejercicio 13. 
Escriba un dfd que escriba el siguiente dibujo.
#### 1.1 Analisis. 
Desarrollar el siguiente diagrama de flujo.



#### 1.2 DFD
![14](https://user-images.githubusercontent.com/113395327/197684075-b7439c57-f658-44ec-b8d3-cb3a0f734614.png)
#### 1.3 Prueba de escritorio 
|i  |i<=5|j  |j<=i|1     |i++ |j++ |
|---|----|---|----|------|----|----|
|1  |1<=5|1  |1<=1|1     |1   |1   | 
|2  |2<=5|2  |2<=2|11    |2   |2   |
|3  |3<=5|3  |3<=3|111   |3   |3   |
|4  |4<=5|4  |4<=4|1111  |4   |4   |
|5  |5<=5|5  |5<=5|11111 |5   |5   |

#### 1.4 Entradas.
No tiene ninguna entrada
#### 1.5 Salidas.
 *
#### 1.6 Codigo.
```dart
import 'dart:io';
void main() {
  var n = 5;
  for (var i = 1; i <= 5; i++) {
    for (var j = 1; j <= i; j++) {
      stdout.write('*');
    }
    print('');
  }
}
```
