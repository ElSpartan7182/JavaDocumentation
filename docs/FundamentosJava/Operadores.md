# Operadores de Java

Como dice su nombre, estos sirven para hacer operaciones entre valores y variables.

Entre ellos, existen varios tipos.
1. Aritméticos
2. De asignación
3. Comparativos
4. Lógicos
5. Bitwise

## Aritméticos

|Operador|Nombre|Descripcion|Ejemplo|
|--------|------|-----------|-------|
|+|Adición|Suma 2 números|a+b|
|-|Substracción|Resta 2 números|a-b|
|*|Multiplicación|Multiplica 2 números|a*b|
|/|División|Divide 2 números|a/b|
|%|Residuo|Regresa el residuo de una división|a%b|
|++|Incremento|Incrementa un valor en 1|x++|
|--|Decremento|Decrese un valor en 1|x--|

Ejemplo en código en main():
```java
int a = 7;
int b = 3;

System.out.println(a+b); // 10
System.out.println(a-b); // 4
System.out.println(a*b); // 21
System.out.println(a/b); // 2
System.out.println(a%b); // 1

a++
System.out.println(a); // 8
b--
System.out.println(b) // 3;
```

## De asignación

|Operador|Ejemplo|Equivalencia|
|--------|-------|------------|
|=|x = 5|x = 5|
|+=|x += 5|x = x + 5|
|-=|x -= 5|x = x - 5|
|*=|x *= 5|x = x * 5| 
|/=|x /= 5|x = x / 5|
|%=|x %= 5|x = x % 5|
|&=|x &= 5|x = x & 5|
|\|=|x \|= 5|x = x \| 5|
|^=|x ^= 5|x = x ^ 5|
|>>=|x >>= 5|x = x>>5|
|<<=|x <<= 5|x = x<<5|

## Comparativos

## Lógicos

## Bitwise