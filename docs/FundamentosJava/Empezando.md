# Empezando de 0

Para los tutoriales que voy a mostrar, ya sean archivos o simples líneas de código, las vas a poder ejecutar al instalar [Visual Studio Code](https://code.visualstudio.com).

**Visual Studio Code** (VSC) es un editor de código bastante versátil, ya que permite desarrollar aplicaciones con prácticamente cualquier lenguaje de programación.

Ahora, ya que tengan Visual Studio instalado, deberán descargar la extensión de Java para que puedan editar código de este de manera más fácil. Eso sí, preferiblemente, instalen también **java** en su computadora.

En el caso de que lo hayan instalado todo correctamente, generen un nuevo proyecto con terminación en `.java` para así poder imprimir su primer `Hello World!`

**Nota: **Para saber si se instaló correctamente, habran una terminar el Visual Studio con ctrl+ñ y escriban `java -version`.
En el caso que les salga algo de java version "x.x.x" entonces está instalado correctamente

## Mi primer Hello World! :)

Se darán cuenta que en lenguajes como **python**, imprimir un **Hello World!** Es bastante sencillo, ya que solo tienen que escribir `print("Hello World!")`

Por otro lado, recordemos que **java** es un *lenguaje de programación orientado a objetos**, por lo que esto no funcionará de esta manera.

- **print:** Print es un método que sirve para mostrar algún texto en la consola como salida, o, en este caso, la terminal.

- **println:** Println es un print con un ln al final, ¿qué quiere decir **ln**? Es la abreviatura de *line*, por lo que, va a mostrar el texto en la consola y además va a agregar un salto de línea.

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
