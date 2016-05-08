---
currentMenu: sequential
---

# Estructuras Secuenciales

En este capítulo aprenderás a distinguir y usar 3 estructuras secuenciales:

* la **asignación**,
* la **lectura** o **entrada** de datos,
* la **salida** de datos.

## Definicion

La estructura secuencial es aquella en la que una acción (instrucción) sigue a
otra en secuencia. Las tareas se suceden de tal modo que la salida de una es la
entrada de la siguiente y así sucesivamente hasta el fin del proceso. Una
estructura secuencial se representa de la siguiente forma:

```
accion 1
accion 2
.
.
accion n
```

## Asignación

La asignación consiste, en el paso de valores o resultados a una variable. Las
asignaciones se pueden clasificar de la siguiente forma:

-   **Simples** Consiste en pasar un valor constante a una variable (`a = 15`)
-   **De trabajo** Donde se recibe el resultado de una operación que
    involucra varias variables o valores (`a = c + b * 2 / 4`).
-   **Contador** Consiste en usar una variable para contar el número de veces que
    se realiza un proceso (`a = a + 1`)
-   **Acumulador** Consiste en usar una variable para acumular un valor en un
    proceso que se puede repetir varias veces (`a = a + b`).

## Lectura

La lectura consiste en recibir desde un dispositivo de entrada (generalmente, el
teclado y el mouse) un valor. Esta operación se representa en un pseudo código
como sigue:

```
leer valor
```

Donde `valor` es el nombre de la variable que recibirá el valor.

## Escritura

Consiste en mandar por un dispositivo de salida (generalmente, el monitor) un
resultado o mensaje. Este proceso se representa en un pseudocódigo como sigue:

```
escribir "El resultado es:", resultado
```

Donde `"El resultado es:"` es un mensaje que se desea aparezca en la pantalla y
`resultado` es una variable que contiene un valor.

## Problemas Secuenciales

1.  Suponga que un individuo desea invertir su capital en un banco y desea saber
    cuanto dinero ganara después de un mes, si el banco paga a razón de 2%
    mensual.
    ```
    inicio
        escribir "Proporcione el capital invertido: "
        leer capitalInvertido
        ganancia = capitalInvertido * 0.02
        escribir "Su ganancia sera de: ", ganancia
    fin
    ```
2.  Una tienda ofrece un descuento del 15% sobre el total de la compra y un
    cliente desea saber cuanto deberá pagar finalmente por su compra.
    ```
    inicio
        escribir "Cuanto compraste?"
        leer totalCompra
        descuento = totalCompra * 0.15
        pagoFinal = totalCompra - descuento
        escribir "Vas a pagar ", pagoFinal
    fin
    ```
3.  Realizar un algoritmo que calcule la edad de una persona.
    ```
    inicio
        escribir "En que anio naciste?"
        leer anioNacimiento
        escribir "En que anio estamos?"
        leer anioActual
        edad = anioActual - anioNacimiento
        escribir "Tienes", edad, "anios"
    fin
    ```
4.  Un vendedor recibe un sueldo base mas un 10% extra por comisión de sus
    ventas, el vendedor desea saber cuanto dinero obtendrá por concepto de
    comisiones por las tres ventas que realiza en el mes y el total que recibirá
    en el mes tomando en cuenta su sueldo base y comisiones.
    ```
    inicio
        escribir "De cuanto es tu sueldo base? "
        leer sueldoBase
        escribir "De cuanto fue tu primer venta? "
        leer ventaUno
        escribir "De cuanto fue tu segunda venta? "
        leer ventaDos
        escribir "De cuanto fue tu tercer venta? "
        leer ventaTres
        totalVentas = ventaUno + ventaDos + ventaTres
        comisiones = totalVentas * 0.10
        sueldoFinal = sueldoBase + comisiones
        escribir "Vas a recibir de comisiones: ",comisiones
        escribir "Tu sueldo final es de: ", sueldoFinal
    fin
    ```
5.  Un maestro desea saber que porcentaje de hombres y que porcentaje de mujeres
    hay en un grupo de estudiantes.
    ```
    inicio
     escribir "Proporcione la cantidad de mujeres:"
     leer numeroMujeres
     escribir "Proporcione la cantidad de hombres:"
     leer numeroHombres
     totalAlumnos = numeroMujeres + numeroHombres
     porcentajeMujeres = numeroMujeres * 100 / totalAlumnos
     porcentajeHombres = numeroHombres * 100 / totalAlumnos
     escribir "El porcentaje de mujeres es de: ",
              porcentajeMujeres
     escribir "El porcentaje de hombres es de: ",
              porcentajeHombres
    fin
    ```
6.  Un alumno desea saber cual será su calificación final en la materia de
    Algoritmos. Dicha calificación se compone de los siguientes porcentajes: 55%
    del promedio de sus tres calificaciones parciales. 30% de la calificación
    del examen final. 15% de la calificación de un trabajo final.
    ```
    inicio
        escribir "Escriba la calificacion del primer examen: "
        leer calificacion1
        escribir "Escriba la calificacion del segundo examen: "
        leer calificacion2
        escribir "Escriba la calificacion del tercer examen: "
        leer calificacion3
        escribir "Escriba la calificacion del examen final: "
        leer calificacionExamenFinal
        escribir "Escriba la calificacion del trabajo final: "
        leer calificacionTrabajoFinal
        promedioParciales = (calificacion1 + calificacion2 + calificacion3)/3
        porcentajePromedio = promedioParciales * 0.55
        porcentajeExamenFinal = calificacionExamenFinal * 0.30
        porcentajeTrabajoFinal = calificacionTrabajoFinal * 0.15
        calificacionFinal =
            porcentajePromedio + porcentajeExamenFinal +
            porcentajeTrabajoFinal
        escribir "Tu calificacion final es: ", calificacionFinal
    fin
    ```

## Problemas Propuestos

1.  Dada un cantidad en pesos, obtener la equivalencia en dólares,
    asumiendo que la unidad cambiaria es un dato desconocido.
2.  La presión, el volumen y la temperatura de una masa de aire se
    relacionan por la fórmula:
    ```
    masa = (presion * volumen) / (0.37 * (temperatura + 460))
    ```
3.  Calcular el numero de pulsaciones que una persona debe tener por
    cada 10 segundos de ejercicio, si la formula es:
    ```
    numeroPulsaciones = (220 - edad) / 10
    ```
4.  Calcular el nuevo salario de un obrero si obtuvo un incremento del
    25% sobre su salario anterior.
5.  En un hospital existen tres áreas: Ginecología, Pediatría, Traumatología. El
    presupuesto anual del hospital se reparte conforme a la siguiente tabla:

    | Área | Porcentaje del presupuesto |
    | ---- | -------------------------- |
    | Ginecología | 40% |
    | Traumatología | 30% |
    | Pediatría | 30% |

    Obtener la cantidad de dinero que recibirá cada área, para cualquier monto
    presupuestal.
6.  El dueño de una tienda compra un artículo a un precio determinado. Obtener
    el precio en que lo debe vender para obtener una ganancia del 30%.
7.  Todos los lunes, miércoles y viernes, una persona corre la misma ruta y
    cronometra los tiempos obtenidos. Determinar el tiempo promedio que la
    persona tarda en recorrer la ruta en una semana cualquiera.
8.  Tres personas deciden invertir su dinero para fundar una empresa. Cada una
    de ellas invierte una cantidad distinta. Obtener el porcentaje que cada
    quien invierte con respecto a la cantidad total invertida.
9.  Un alumno desea saber cual será su promedio general en las tres materias más
    difíciles que cursa y cual será el promedio que obtendrá en cada una de
    ellas. Estas materias se evalúan como se muestra a continuación:

    La calificación de Matemáticas se obtiene de la siguiente manera:
    -   Examen 90%
    -   Promedio de tareas 10%
    -   En esta materia se pidió un total de tres tareas.

    La calificación de Física se obtiene de la sig. manera:
    -   Examen 80%
    -   Promedio de tareas 20%
    -   En esta materia se pidió un total de dos tareas.

    La calificación de Química se obtiene de la sig. manera:
    -   Examen 85%
    -   Promedio de tareas 15%
    -   En esta materia se pidió un promedio de tres tareas.
