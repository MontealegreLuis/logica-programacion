Subprogramas {#cap:Subprogramas}
============

Definición y Manipulación
-------------------------

Un problema complejo se puede dividir en pequeños subproblemas mas
sencillos. Estos subproblemas se conocen como “Módulos” y su
implementación en un lenguaje se llama subprograma (procedimientos y
funciones).

Un subprograma realiza las mismas acciones que un programa, sin embargo,
un subprograma lo utiliza solamente un programa para un propósito
especifico.

Un subprograma recibe datos de un programa y le devuelve resultados (el
programa “llama” o “invoca” al subprograma, este ejecuta una tarea
especifica y devuelve el “control” al programa que lo llamo). La Figura
[fig:modulos] ilustra la calisificación de los módulos.

### Funciones

Una función en matemáticas, es una operación que toma un o mas valores
(argumentos) y devuelve un resultado (valor de la función para los
argumentos dados). Por ejemplo:

<span>$F(X) = X / (1+ X^2)$</span>

Donde: F es el nombre de la función, x es el argumento (también conocido
como parámetro formal)

La definición de una función se presenta de la siguiente manera:

        tipoValor nombreFuncion (p1, p2, \ldots, pn)
        Inicio
           Bloque de instrucciones
           Retorna valor
        Fin

Donde: tipoValor indica el tipo de valor que devolverá la función.
nombreFuncion es el identificador con el cual se reconoce a la función
en el cuerpo del algoritmo principal. P1,p2,…,pn es el grupo de
parámetros que define a la función. Y valor es el valor que devuelve la
función

Cuando definimos una función solo le indicamos al algoritmo que esta
función existe, pero una definición de función no implica la realización
de las instrucciones que la constituyen. Para hacer uso de una función,
el algoritmo principal la debe llamar. Por ejemplo:

        real F(real X)
        Inicio
            F = X /(1 + X ^2)
        Fin
        Inicio
           Imprimir "Este es el algoritmo principal"
           Leer N
           R = F(N)
           Imprimir "El resultado de la funci\'on es:",R
        Fin

### Problemas Propuestos

1.  Diseñe un algoritmo que llene una matriz de 10 \* 10 y determine:

    -   El numero mayor almacenado en la matriz

    -   El numero mayor almacenado en cada renglón

    -   La columna que tuvo la máxima suma

    -   El renglón que tuvo la máxima suma

    Diseña una función para cada inciso.

2.  Diseñe un algoritmo que lea un numero y mediante una función regrese
    el valor de 1 si el numero es positivo y -1 si es negativo.

[^1]: Antiguamente una memoria ROM no se podía reescribir, actualmente
    contamos con memorias PROM (Reprogramables una sola vez), EPROM (ROM
    Borrable y programable), EEPROM (ROM Borrable y programable
    eléctricamente) y flash (EEPROM que permite borrar varias celdas en
    una sola operación).

[^2]: Mejor conocida como Ada Lovelace

[^3]: Es de aclarar que los procedimientos y/o funciones son bloques de
    instrucciones que forman el cuerpo de un programa y que se
    analizarán a profundidad en el Cap’itulo 5.
