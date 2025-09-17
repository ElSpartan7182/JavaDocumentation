# Empezando de 0

Para los tutoriales que voy a mostrar, ya sean archivos o simples líneas de código, las vas a poder ejecutar al instalar [Visual Studio Code](https://code.visualstudio.com).

**Visual Studio Code** (VSC) es un editor de código bastante versátil, ya que permite desarrollar aplicaciones con prácticamente cualquier lenguaje de programación.

Ahora, ya que tengan Visual Studio instalado, deberán descargar la extensión de Java para que puedan editar código de este de manera más fácil. Eso sí, preferiblemente, instalen también **java** en su computadora.

En el caso de que lo hayan instalado todo correctamente, generen un nuevo proyecto con terminación en `.java` para así poder imprimir su primer `Hello World!`

**Nota: **Para saber si se instaló correctamente, habran una terminar el Visual Studio con ctrl+ñ y escriban `java -version`.
En el caso que les salga algo de java version "x.x.x" entonces está instalado correctamente

## Mi primer Hello World! :)

Se darán cuenta que en lenguajes como **python**, imprimir un **Hello World!** Es bastante sencillo, ya que solo tienen que escribir `print("Hello World!")`

Por otro lado, recordemos que **java** es un **lenguaje de programación orientado a objetos**, por lo que esto no funcionará de esta manera.

- **print:** Print es un método que sirve para mostrar algún texto en la consola como salida, o, en este caso, la terminal.

- **println:** Println es un print con un **ln** al final, ¿qué quiere decir **ln**? Es la abreviatura de *line*, por lo que, va a mostrar el texto en la consola y además va a agregar un salto de línea.

Voy a mostrar un pequeño código para imprimir `Hello World!` y lo vamos explicando paso a paso!

```java
class Main {
    public static void main(String[] args) {
        System.out.print("Hello World!");
    }
}
``` 

Como podemos observar, son más líneas de código a diferencia de **python**, pero viéndolo bien, realmente no es mucho.

1. `class` Significa **clase**
2. `Main` Es el nombre de la clase
3. `public static void main(String[] args)` Es el método principal de la clase, el cual ejecuta **TODO** el programa
4. `System.out.print("Hello World!");` Es el método que imprime el texto

Solo son 4 puntos clave, pero fundamentales.
No te preocupes si todavía no entiendes los conceptos que acabo de mencionar, pero es importante que sepas como compilar y ejecturar este código.

Si instalaste correctamente los programas para java, y pusiste este código en un archivo llamado `Main.java`, entonces abre una terminal con **ctrl+ñ** y escribe `javac Main.java`. Eso va a **compilar** el programa para verificar que no hayan errores. Una vez que no hayan errores, escribe `java Main` para ejecutar el código. Una vez que lo ejecutaste, en tu consola o terminar deberá aparecer `Hello World!`

## Explicación del ejemplo

El ejemplo que había mostrado para hacer el primer **Hello World!** es el siguiente:

```java
class Main {
    public static void main(String[] args) {
        System.out.print("Hello World!");
    }
}
``` 

Pero... ¿Qué significa cada cosa?

Para resolver esta pregunta debemos recordar que estamos utilizando un **lenguaje de programación orientado a objetos**, por lo que, todo el código deberá estar dentro de una **clase**. En el caso de que la clase sea la principal, deberá empezar con **mayúscula**, en este caso, `Main` es la clase principal. Eso sí, el nombre de la clase principal deberá tener **el mismo nombre** que el archivo. Si tu archivo se llama `Test.java` entonces tu clase principal deberá llamarse `class Test`

**Importante:** Java es un lenguaje que distingue las mayúsculas de las minúsculas, por lo que `Clase1` y `clase1` son diferentes.

Ahora, sigamos con el método principal del programa que es: `public static void main(String[] args)`

Todas las líneas de código que pongamos dentro del método `main()`serán ejecutadas. 

**Nota:** las palabras como `public`, `static`, y `void` las vamos a estar viendo poco a poco :)

Luego, tenemos `System.out.print("Hello World!");`

Esta línea de código se encuentra dentro del **método** `main()` ya que queremos que se ejecute. Simplemente imprimimos una línea de texto en la consola o terminal.

**Nota:** Todas las **líneas de código** deben de terminar con un punto y coma `;` y cada bloque de texto se encuentra dentro de llaves `{}`

## ¿Qué es System?

`System`en java es una clase integrada que nos da acceso a varias funciones del **sistema** como el **input**(entrada) y **salida**(output). Existe el `System.in`, `System.out`y `System.err` que son **variables estáticas** dentro de la clase **System**.

Este viene de un **paquete** llamado `java.lang`. Ya veremos más adelante los detalles de estas descripciones, pero es bueno tener una panorámica de lo que se va a trabajar.

Recuerden definiciones como `InputStream` y `PrintStream`, ya que el primero se relaciona con `System.in` y el segundo con `System.out` :)

## Print()

Ya hablamos de las funciones `print()` y `println()`, pero, no hemos visto varias de sus propiedades.

1. Los métodos `print()` o `println()`, pueden escribirse varias veces en el código y van a imprimir los textos que le indiques.

```java
System.out.println("Hello World!);
System.out.println("Hola Mundo");
System.our.println("Texto 3");
```

El output se vería así:
```java
Hello World!
Hola Mundo
Texto 3
```

Pero si colocamos `print()` en vez de `println()`:
```java
System.out.print("Hello World!);
System.out.print("Hola Mundo");
System.our.print("Texto 3");
```

El output se vería así:
```java
Hello World!Hola MundoTexto 3
```

**Nota:** Recuerda colocar tu texto en comillas dobles **" "** 

Por último, `print()` también sirve para imprimir números.

```java
System.out.print(1);
```

El output se vería: `1`

Pero también podemos imprimir **operaciones matemáticas**, aquí te dejo 5 básicas.

1. Suma: **+**
2. Resta: **-**
3. Multiplicación: **\**
4. División: **/**
5. Módulo: **%**

Esto quiere decir que si ponemos

```java
System.out.print(5 + 5);
```
El output se vería: `10`

Por último, existe el `printf()` que significa **print format**. Por el momento no hablaremos tanto, ya que requiere de cierto conocimiento un poquito avanzado, pero más adelante veremos de que trata.

## Comentarios en Java

Los comentarios sirven para dar alguna explicación, por ejemplo, si alguien externo ve tu código, leyendo los comentarios va a poder darse una idea más rápido que andar leyendo línea por línea el funcionamiento.

**Pequeño tip:** Si escribes algún código nuevo que no funciona, puedes ponerlo en comentarios para que no afecte el demás código ;)

Podemos poner líneas sencillas de comentarios con `//`. Las puedes poner sobre líneas de código o terminando estas
Ejemplo:
```java
// Esto es un comentario encima de una línea
System.out.print("Hola!"); // Este es otro comentario al terminar la línea
```

También tenemos comentarios de varias líneas. Estas empiezan con `/*` y terminan con `*/`, así que, todo el texto que incluyan dentro de esas se considerarán comentario.

```java
/* Estas son varias líneas de comentarios,
que pueden ser muy largas y explicar de manera más extensa */

System.out.print("Hola!");
```

Por último, tenemos las líneas de código de "Documentación", estas se colocan para especificar variables y explicar de manera extensa. Para usarlas, tienes que poner `/**` y luego `enter` para que se genere y puedas escribir algo como esto:

```java
/**
 * @param AsiSeEspecificaAlgunaVariable y la podemos explicar
 * Y luego explicamos otras cosas
*/

System.out.println("Son muy útiles :O");
```