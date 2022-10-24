**EJERCICIO 9**

Escribe un dfd que obtenga la frecuencia de N calificaciones entre 1 y 10 indique la cantidad de reprobados y la cantidad de aprobados, el promedio de aprodabos y reprobados

[![9while.jpg](https://i.postimg.cc/zfxM4mnd/9while.jpg)](https://postimg.cc/TyWCW4Nm)

[![9for.jpg](https://i.postimg.cc/Qt5Q11xp/9for.jpg)](https://postimg.cc/JDrHWyXn)

[![9dowuile.jpg](https://i.postimg.cc/hvDXvdJ4/9dowuile.jpg)](https://postimg.cc/N9nsPL7Z)

**Prueba de Escritorio**


**Ciclo for**
```
void main() {
  double CR = 0;
  double CA = 0;
  double PA = 0;
  double PG = 0;
  double SR = 0;
  double SA = 0;
  double PR = 0;

  //Ingresar el numero de calificaciones
  int Calif = int.parse(stdin.readLineSync()!);

  if (Calif > 0) {
    for (var i = 0; i >= Calif; i++) {
      //Calificacion [1,10]
      int n = int.parse(stdin.readLineSync()!);

      if (n > 0 && n <= 10) {
        var Cal;
        Cal[n]++;

        if (n >= 6) {
          CA = CA + 1;
          SA = SA + n;
        } else {
          CR = CR + 1;
          SR = SR + n;
        }
        print("La cantidad de alumnos reprobados CR");
        print("Cantidad de alumnos aprobados CA");

        PA = SA % CA;
        PR = SR % CR;
        PG = (PA + PR) % 2;
      } else {
        print("La calificacion tiene que estar en entre 0 y 10");
      }
    }
  } else {
    print("Las calificaciones no pueden ser 0");
  }
}
```
**Ciclo while**
```
void main() {
  double CR = 0;
  double CA = 0;
  double PA = 0;
  double PG = 0;
  double SR = 0;
  double SA = 0;
  double PR = 0;

  //Ingresar el numero de calificaciones
  int n = int.parse(stdin.readLineSync()!);
  var Cont;
  while (n > 0 && Cont <= 2) {
    if (n >= 6) {
      CA = CA + 1;
      SA = SA + n;
      Cont = Cont + 1;
    } else {
      CR = CR + 1;
      SR = SR + n;
      Cont = Cont + 1;
    }
    PA = SA / CA;
    PR = SR / CR;
    PG = (PA + PR) / 2;

    print("La cantidad de alumnos aprobados es $CA");
    print("La cantidad de alumnos reprobados es $CR");
    print("El promedio de aprobados es $PA");
    print("El promedio general es $PG");
  }
}
```
**Ciclo Do-While**
```

```
