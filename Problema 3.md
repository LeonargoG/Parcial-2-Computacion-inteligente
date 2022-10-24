**EJERCICIO 3**

Escribe un DFD que 

[![3-ER-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/9MTZGJkb/3-ER-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/ZBbWmF4v)

[![3-ER-PROBLEMA-FOR.jpg](https://i.postimg.cc/vHGfV7t7/3-ER-PROBLEMA-FOR.jpg)](https://postimg.cc/rzYD6rbz)

[![3-ER-PROBLEMA-WHILE.jpg](https://i.postimg.cc/d18Z7D7S/3-ER-PROBLEMA-WHILE.jpg)](https://postimg.cc/S2xx3SfW)

|Corrida|Contador/posicion en el array|Numero ingresado|
|-|-|-|
|1|0|5|
|2|1|5|
|3|2|5|
|4|3|5|

Ejemplo del array

|5|
|-|
|5|
|5|
|5|

**Entradas= 1**

**Salidas=1**

**Ciclo for**
```
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
**Ciclo While**
```
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
**Ciclo Do-While**
```
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```
