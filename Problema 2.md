**EJERCICIO 2**

Realiza un DFD que obtenga la suma de los primeros 5 numeros pares

[![2-DO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/4nRJKBgt/2-DO-PROBLEMA-WHILE.jpg)](https://postimg.cc/V04yp95L)

[![2-DO-PROBLEMA-FOR.jpg](https://i.postimg.cc/Vk1CpFCd/2-DO-PROBLEMA-FOR.jpg)](https://postimg.cc/hfyv7TMB)

[![2-DO-PROBLEMA-DO-WHILE.jpg](https://i.postimg.cc/7LtJC8Q2/2-DO-PROBLEMA-DO-WHILE.jpg)](https://postimg.cc/VSMkTTwf)

**Prueba de Escritorio**

|Corridas|C|S+C*2|S|
|-|-|-|-|
|1|1|0+2|2|
|2|2|2+2|4|
|3|3|4+6|10|
|4|4|10+8|18|
|5|5|18+10|28|

**Entradas=0**

**Salidas=1**

**Ciclo for**

```
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```
**Ciclo while**

```
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```
**Ciclo Do-while**

```
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
}
```
