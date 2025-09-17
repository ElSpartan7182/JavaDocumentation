# Casting de Java

## ¿Qué significa Casting?

El **Casting** es cuando quieres convertir algún tipo de dato primitivo en otro. Es decir, si quieres convertir un `int` en un `double` o viceversa, se utiliza el **Casting**

## Tipos de Casting

En Java existen 2 tipos de **Casting**:

1. **Widening Casting:** Este tipo de **Casting** es cuando quieres pasar de un tipo de dato pequeño a uno grande. El orden de los tipo de datos de más pequeño a más grande es:
    - byte
    - short
    - char
    - int
    - long
    - float
    - double

Ejemplo de uso en main():
```java
int x = 1;
double y = x; // Ya se hizo un Casting

System.out.println(x); // Sale 1
System.out.println(y); // Sale 1.0
```

2. **Narrowing Casting:** Este otro tipo es cuando quieras pasar de un tipo de dato pequeño a uno grande, por lo que, el orden de más grande a más pequeño es:
    - double
    - float
    - long
    - int
    - char
    - short
    - byte

Ejemplo de uso en main():
```java
double num = 9.2;
int x = (int)num; // Se aplico un Casting manual

System.out.println(num); // Sale 9.2
System.out.println(x); // Sale 9
```