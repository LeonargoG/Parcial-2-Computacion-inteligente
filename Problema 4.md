**Ejercicio 4**

Escribe un dfd que almacene los N numeros leidos del teclado en el vector de 10

[![4-TP-PROBLEMA-WHILE.jpg](https://i.postimg.cc/RhN4nDhp/4-TP-PROBLEMA-WHILE.jpg)](https://postimg.cc/BP9drNx2)

[![4-TP-PROBLEMA-FOR.jpg](https://i.postimg.cc/8PfTp9qj/4-TP-PROBLEMA-FOR.jpg)](https://postimg.cc/hfnkMy4B)

[![4-TP-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/d1SKvj62/4-TP-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/2bvt7vPy)

**Prueba de escritorio**

|Corrida|Contador|Numeros usados|Numero ingresado|
|-|-|-|-|
|1|0|1|5|
|2|1|2|7|
|3|2|3|8|

Ejemplo del array 

|5|
|-|
|7|
|8|

**Codigo**
```dart
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
