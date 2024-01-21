# MUSE/NLP 

Muse es un lenguaje que te permite usar las notas musicales para dar órdenes al ordenador. Así puedes hacer que el ordenador haga sonidos, dibujos, juegos y mucho más.

Para que entiendas mejor cómo funciona Muse, te voy a explicar algunas partes de tu código como si fueras un niño de 5 años. No te preocupes, no es difícil. Solo tienes que prestar atención y seguir los pasos.

## Cómo imprimir "¡Hola, mundo!"

```nlp
inicio
    imprimir("¡Hola, mundo!")
fin
```

Esta parte del código es muy sencilla. Lo que hace es decirle al ordenador que empiece a hacer algo (`inicio`) y que termine de hacerlo (`fin`). Entre esas dos palabras, le decimos lo que queremos que haga. En este caso, le decimos que imprima o escriba en la pantalla el texto "¡Hola, mundo!" (`imprimir("¡Hola, mundo!")`). Así el ordenador nos saluda y nos muestra que está listo para seguir nuestras órdenes.

## Cómo usar notas como variables

```nlp
# Definir las notas como variables
C = "Instrucción 1"
D = "Instrucción 2"
E = "Instrucción 3"

# Ejecutar las instrucciones según las notas
nota_actual = C
print(nota_actual)  # Output: Instrucción 1

nota_actual = D
print(nota_actual)  # Output: Instrucción 2

nota_actual = E
print(nota_actual)  # Output: Instrucción 3
```

Esta parte del código es un poco más complicada, pero no te asustes. Lo que hace es usar las notas musicales como variables. ¿Qué son las variables? Son como cajitas donde guardamos cosas que queremos usar después. Por ejemplo, podemos guardar una pelota en una caja y ponerle el nombre de "pelota". Así, cuando queramos jugar con la pelota, solo tenemos que decir "pelota" y el ordenador sabrá que nos referimos a la caja que tiene la pelota dentro.

En este caso, usamos las notas C, D y E como variables. Les ponemos esos nombres porque son las primeras letras del alfabeto musical. Dentro de cada nota guardamos una instrucción, que es lo que queremos que haga el ordenador. Por ejemplo, en la nota C guardamos la instrucción 1, en la nota D guardamos la instrucción 2 y en la nota E guardamos la instrucción 3. Así, cuando queramos que el ordenador haga una de esas instrucciones, solo tenemos que decirle la nota que la contiene.

Para hacer eso, usamos otra variable llamada nota_actual. Esta variable es como una caja vacía que podemos llenar con la nota que queramos. Por ejemplo, si queremos que el ordenador haga la instrucción 1, le decimos que nota_actual es igual a C (`nota_actual = C`). Así, la caja de nota_actual se llena con la caja de C, que tiene dentro la instrucción 1. Luego, le decimos al ordenador que imprima o escriba en la pantalla lo que hay dentro de nota_actual (`print(nota_actual)`). Así, el ordenador nos muestra la instrucción 1. Podemos hacer lo mismo con las otras notas e instrucciones.

## Cómo usar notas como argumentos de funciones

```nlp
# Definir funciones que ejecutan instrucciones según la nota
def instruccion_nota(nota):
    if nota == "C":
        print("Instrucción 1")
    elif nota == "D":
        print("Instrucción 2")
    elif nota == "E":
        print("Instrucción 3")

# Llamar a la función con diferentes notas
instruccion_nota("C")  # Output: Instrucción 1
instruccion_nota("D")  # Output: Instrucción 2
instruccion_nota("E")  # Output: Instrucción 3
```

Esta parte del código es un poco más avanzada, pero no te preocupes. Lo que hace es usar las notas musicales como argumentos de funciones. ¿Qué son los argumentos y las funciones? Los argumentos son como regalos que le damos al ordenador para que haga algo con ellos. Las funciones son como máquinas que reciben los regalos y los transforman en algo diferente. Por ejemplo, podemos tener una función que se llama sumar, que recibe dos números como argumentos y los suma. Así, si le damos a la función sumar los números 2 y 3, nos devuelve el número 5.

En este caso, tenemos una función que se llama instruccion_nota, que recibe una nota musical como argumento y ejecuta la instrucción que corresponde a esa nota. Por ejemplo, si le damos a la función instruccion_nota la nota C, nos devuelve la instrucción 1. Para hacer eso, la función usa unas palabras que se llaman `if`, `elif` y `else`. Estas palabras sirven para hacer preguntas al ordenador y darle opciones de respuesta. 

Por ejemplo, la función le pregunta al ordenador si la nota que le dimos es igual a C (`if nota == "C"`). Si la respuesta es sí, le dice que imprima o escriba en la pantalla la instrucción 1 (`print("Instrucción 1")`). Si la respuesta es no, le pregunta si la nota que le dimos es igual a D (`elif nota == "D"`). Si la respuesta es sí, le dice que imprima o escriba en la pantalla la instrucción 2 (`print("Instrucción 2")`). Si la respuesta es no, le pregunta si la nota que le dimos es igual a E (`elif nota == "E"`). Si la respuesta es sí, le dice que imprima o escriba en la pantalla la instrucción 3 (`print("Instrucción 3")`). Si la respuesta es no, no hace nada.

Para usar la función, solo tenemos que escribir su nombre y entre paréntesis la nota que queremos que reciba como argumento. Por ejemplo, si queremos que la función ejecute la instrucción 1, escribimos `instruccion_nota("C")`. Así, le damos a la función la nota C como regalo y nos devuelve la instrucción 1. Podemos hacer lo mismo con las otras notas e instrucciones.

## Cómo usar notas para controlar el flujo del programa

```nlp
# Definir una lista de notas
melodia = ["C", "D", "E"]

# Ejecutar instrucciones según las notas en la lista
for nota in melodia:
    if nota == "C":
        print("Instrucción 1")
    elif nota == "D":
        print("Instrucción 2")
    elif nota == "E":
        print("Instrucción 3")
```

Esta parte del código es la más difícil, pero no te rindas. Lo que hace es usar las notas musicales para controlar el flujo del programa. ¿Qué es el flujo del programa? Es el orden en el que el ordenador hace las cosas que le decimos. A veces queremos que el ordenador haga las cosas una por una, y otras veces queremos que las haga varias veces o que las cambie según lo que pase. Para hacer eso, usamos unas palabras que se llaman for, while, break, continue, etc. Estas palabras sirven para repetir, parar o saltar las cosas que queremos que haga el ordenador.

En este caso, usamos la palabra for para repetir las instrucciones según las notas que hay en una lista. ¿Qué es una lista? Es como una fila de cajas donde guardamos cosas que queremos usar después. Por ejemplo, podemos guardar las notas C, D y E en una lista y ponerle el nombre de melodia (`melodia = ["C", "D", "E"]`). Así, tenemos una fila de tres cajas que tienen dentro las notas C, D y E.

Para usar la lista, usamos la palabra for y le decimos al ordenador que tome cada nota de la lista y la guarde en una variable llamada nota (`for nota in melodia`). Así, el ordenador va tomando una por una las notas de la lista y las guarda en la caja de nota. Luego, le decimos al ordenador que ejecute la instrucción que corresponde a la nota que tiene en la caja de nota, usando las palabras if, elif y else que ya vimos antes. Así, el ordenador va haciendo las instrucciones según las notas que hay en la lista, una tras otra.

## Cómo hacer más ejemplos de código

Estas son solo algunas partes de tu código que te he explicado como si fueras un niño de 5 años. Hay muchas más cosas que puedes hacer con Muse, como crear acordes, melodías, armonías, etc. Para aprender más sobre Muse, te recomiendo que visites:

1. [Cómo poner límites y normas a los niños de 5 años sin desesperarse] (https://www.guiainfantil.com/educacion/limites/como-poner-limites-y-normas-a-los-ninos-de-5-anos-sin-desesperarse/) 
2. [¿Cómo Estimular el Desarrollo de un Niño de 5 Años?](https://www.tuconducta.com/guia-infantil/actividades-de-estimulacion-para-ninos-de-5-anos) 
3. [Código Morse para niños | Madres Hoy](https://bing.com/search?q=c%c3%b3mo+explicar+el+c%c3%b3digo+a+un+ni%c3%b1o+de+5+a%c3%b1os) 
4. [Código Morse para niños | Madres Hoy](https://madreshoy.com/codigo-morse-para-ninos/) 
