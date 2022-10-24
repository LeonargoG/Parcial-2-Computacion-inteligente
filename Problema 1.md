**EJERCICIO 1**

DFD Que cuente del 1 al 10 y sume los valores

[![1-ER-PROBLEMA-FOR.jpg](https://i.postimg.cc/VN1fR72k/1-ER-PROBLEMA-FOR.jpg)](https://postimg.cc/21cNjxzs)

[![1-ER-PRBLEMA-WHILE.jpg](https://i.postimg.cc/FKZ9nyQg/1-ER-PRBLEMA-WHILE.jpg)](https://postimg.cc/B8j9j1bX)

[![1-ER-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/RFpvvvhW/1-ER-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/R6tkR5cm)

**Prueba de escritorio**

|Corridas|S|C/i|Resultado(s+c/i)|
|-|-|-|-|
|1|0|1|1|
|2|1|2|3|
|3|3|3|6|
|4|6|4|10|

**Entradas= 0**

**Salidas= 1**

**Ciclo for**

```
void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
**_Ciclo while:_**
```
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
```
**_Ciclo do-while:_**
```
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
```
