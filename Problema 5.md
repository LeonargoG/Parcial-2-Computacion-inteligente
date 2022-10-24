**EJERCICIO**

Escribe un dfd que almacene un contador negativo del 10 al 0 en un vector

[![5-TO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/bNPZsQjx/5-TO-PROBLEMA-WHILE.jpg)](https://postimg.cc/s1njLGxx)

[![5-TO-PROBLEMA-FOR.jpg](https://i.postimg.cc/26v555c9/5-TO-PROBLEMA-FOR.jpg)](https://postimg.cc/VrfwGzcX)

[![5-TO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/kGmgRdLJ/5-TO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/62MXFF9g)

**Prueba de escritorio**

|Corrida|Contador|Posicion del vector|Numero asignado al vector|
|-|-|-|-|
|1|10|0|10|
|2|10|1|9|
|3|9|2|8|

**Ejemplo del array**

|10|
|-|
|9|
|8|
|7|
|6|

**Ciclo For**
```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
**Ciclo while**

```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
}
```

**Ciclo Do-While**
```
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```
