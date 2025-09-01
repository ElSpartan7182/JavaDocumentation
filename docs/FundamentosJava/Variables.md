# Variables en Java y tipos de datos

## ¿Qué son las variables?

Las variables son espacios de almacenamiento en la memoria para guardar algún tipo de dato.

En pocas palabras, son cajas ordenadas para guardar algo. No puedes guardar un texto en una caja de números, tienes que ponerla en una caja para textos :)

## Datos primitivos

### ¿Qué son los datos primitivos?

Ya hablamos que las variables pueden almacenar tipos de datos, pero existen unos datos que son los más comunes por asi decirlo, y estos son los que más se utilizan. Hablo de los datos primitivos.

### ¿Cuáles son?
- `int`: almacena números enteros.
- `double`: almacena números enteros y decimales.
- `boolean`: almacena **true** y **false**.
- `char`: almacena un caracter en **Unicode** o valores **ASCII**.
- `byte`: almacena números enteros.
- `short`: almacena números enteros.
- `long`: almacena números enteros.
- `float`: almacena números enteros y decimales.

Aquí te dejo una tabla con algunas cosas importantes que debes considerar de estos tipos de datos.


| Tipo de dato | Tamaño en la memoria | Valor mínimo (decimal aproximado) | Valor máximo (decimal aproximado) |
| ------------ | -------------------- | ------------ | ------------ |
| boolean | 1 bits | false | true |
| byte | 8 bits | -128 | 127 |
| short | 16 bits | -32,768 | 32,767 |
| char | 16 bits | \u000 | \ufff |
| int | 32 bits | -2,147,483,648 | -2,147,483,647 |
| float | 32 bits | -3.4028235x10^38 | 3.4028235x10^38 |
| long | 64 bits | -9,223,372,036,854,775,808 | 9,223,372,036,854,775,807 |
| double | 64 bits | -4.9406564584124654 × 10^-324 | 2.2250738585072014 × 10^308 |

## Establecer variables

El método para establecer una variable es el siguiente:
`tipoDeDato` `nombreDeVariable` = `valorDeVariable`

Ahora, para ponerle nombre a tus variables hay que saber lo siguiente:

1. El nombre de la variable puede contener letras, números, guiones bajos y signos de dinero.

2. Las variables **deben** empezar en una letra.

3. La letra con la que empieza debe estar en minúscula y no puede contener algún espacio.

4. Esto contradice el 2, pero las varibles pueden empezar con **$** o **_**.

5. Las mayúsculas y minúsculas afectan a las variables, es decir, `miVariable` y `mivariable` no es lo mismo.

6. Palabras como los tipos de datos no pueden usarse como nombre, e.j: `int int = 1` no es posible.

Un ejemplo claro es el siguiente: `int numero = 1` donde `int` es el tipo de dato, `numero` es el nombre de la variable y `1`es el valor de esta.

Hasta ahora, ya conoces los tipos de datos primitivos, por lo que puedes jugar con ellos y establecer variables.

## Recomendaciones

Una recomendación para que puedan mantener el orden y la comprensión de su código, es nombrar las variables con su tipo de dato, y/o con el dato que almacenan.

### ¿Qué se puede hacer con las variables?

- **Imprimir el valor de la variable:** Si declaras una variable y la colocas dentro de un `print()`, se va a imprimir el valor de esta.
**Ejemplo en main():**
```java
int x = 1;
System.out.print(x); // En la consola verás 1
```

- **Reestablecer el valor de la variable:** Puedes modificar el valor interno de la variable, siempre y cuando no tenga un `final`.
**Ejemplo en main():**
```java
int x = 1;
x = 2;

System.out.print(x); // En la consola verás 2
```

- **Poner un valor fijo:** Ya hablamos del `final`, este sirve para fijar un valor en una variable, en el caso de que lo quieras reestablecer, te dará un error.

El `final` es como si dijeramos valor **final** de la variable. Se utiliza para dar valores que simplemente no cambian, por ejemplo: una hora son 60 minutos.
**Ejemplo en main():**
```java
final int x = 1;
x = 2; // Esto genera un error
```

- **Operaciones:** Puedes usar operadores aritméticos para los tipos de variables que guardan algún número.
**Ejemplo en main():**
```java
int x = 1+2; // Esto es una suma dentro de una variable

int y = 1;
int z = 2;

int suma = y+z; // Esta es una suma de variables
```

## Otros tipos de datos

Existen tipos de datos que **NO** son primitivos, por ejemplo los **Strings, Arrays, Clases, etc**

En este momento sólamente hablaremos un poco de los Strings.

### Strings

Los `String` son un tipo de dato, que a pesar de no ser un dato primitivo, es uno de los tipos de datos más utilizados. Estos almacenan cadenas de texto dentro de 2 comillas `" "`

Una forma de establecer una variable de String sería algo así: `String nombre = "Nombre de persona";`

#### Largo de un String

String() en Java es prácticamente un objeto, por lo que tiene **propiedades** o mejor dicho, **métodos**. Una de ella es su tamaño. Cuando queremos saber la cantidad de caracteres que tiene la cadena de texto, utilizamos la propiedad `length()`. 

Es importante que cuando hablamos de cantidad, hablamos de un **número**, por lo que, esta propiedad la podemos almacenar en una variable de tipo `int`.

**Ejemplo en main():**
```java
String saludo = "Hola! ¿Cómo estás?";

int x = saludo.length();

System.out.println(x); // Imprime la cantidad de caracteres (18)
```

#### Mayusculas y Minusculas

Si queremos hacer un texto en mayúsuculas o minúsculas, podemos usar los métodos `toUpperCase()` o `toLowerCase()`.

```java
String prueba = "Hola Persona";
String pruebaMayusculas = prueba.toUpperCase();
String pruebaMinusculas = prueba.toLowerCase();

System.out.println(pruebaMayusculas); // Imprime HOLA PERSONA
System.out.println(pruebaMinusculas); // Imprime hola persona
```

#### Encontrar un caracter

Si ahora, queremos saber cuál es la posición de algún caracter o la posición inicial de alguna palabra, podemos utilizar el método `indexOf()`.

**Ejemplo en main();**
```java
String texto = "Este es un texto de prueba";
System.out.println(texto.indexOf("texto")); // El output es 11
```

#### Suma de un String

Los String, también tienen la peculiaridad de que se pueden sumar, ¿de qué manera?, pues... Supongamos que tienes un texto que dice `Hola` y le sumas `Mundo`, el resultado de eso, sería `HolaMundo`. Esta propiedad de los String se conoce como **concatenación**

**Ejemplo en main():**
```java
String nombre = "Carlos";
String apellido = "Flores";

System.out.println(nombre + " " + apellido); //Esto imprime Carlos Flores
```

#### Numeros en los Strings

Los números, también pueden encontrarse dentro de los Strings, por ejemplo, puedes sumar números y Strings.
Eso sí, hay que considerar que se suman como strings, por lo que sumar `1` y `2` en forma de String, resultaría como **12**.

- **Ejemplo en main():**
```java
int num = 3;
String num1 = "1";
String num2 = "2";

System.out.println(num + num1); //Esto imprime 31
System.out.println(num1 + num2); //Esto imprime 12
```

#### Casos especiales

¿Qué pasaría si quisieran poner comillas en un String? Es decir, `"Hola, el termino "Hola" es el principio de este enunciado"`
Básicamente te daría un error. ¿Cómo evitarlo? Ponle un `\` antes de las comillas.

En la siguiente tabla explicaré los siguiente:

|Carácter que da error| Forma de evitarlo |
| - | - |
|" "| \" |
|' '| \' |
| \ | \\\ |

Aquí dejo otras secuencias útiles para los textos de los Strings:

| Forma útil | Lo que hace |
| ---------- | ----------- |
| \n | Es un **enter**|
| \t | Espacio de **tabulador**|
