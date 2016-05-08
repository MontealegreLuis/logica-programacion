---
currentMenu: subprograms
---

# Subprogramas

## Definición y Manipulación

Un problema complejo se puede dividir en pequeños subproblemas más sencillos.
Estos subproblemas se conocen como "Módulos" y su implementación en un lenguaje
se llama subprograma (procedimientos y funciones).

Un subprograma realiza las mismas acciones que un programa, sin embargo, un
subprograma se utiliza únicamente un programa para un propósito específico.

Un subprograma recibe datos de un programa y le devuelve resultados (el programa
"llama" o "invoca" al subprograma, este ejecuta una tarea específica y devuelve
el "control" al programa que lo llamo). La siguiente figura ilustra la
clasificación de los módulos.

![Módulos](images/modulos.png)

### Funciones

Una función en matemáticas, es una operación que toma un o más valores
(argumentos) y devuelve un resultado (valor de la función para los argumentos
dados). Por ejemplo:

<code>f(x) = x / (1+ x<sup>2</sup>)</code>

Donde: `f` es el nombre de la función, `x` es el argumento (también conocido
como parámetro formal)

La definición de una función se presenta de la siguiente manera:

```
tipoValor nombreFuncion (p1, p2, ..., pn)
Inicio
   Bloque de instrucciones
   Retorna valor
Fin
```

Donde: `tipoValor` indica el tipo de valor que devolverá la función.
`nombreFuncion` es el identificador con el cual se reconoce a la función en el
cuerpo del algoritmo principal. `p1, p2, … , pn` es el grupo de parámetros que
define a la función. Y valor es el valor que devuelve la función.

Cuando definimos una función solo le indicamos al algoritmo que esta función
existe, pero una definición de función no implica la ejecución de las
instrucciones que la constituyen. Para hacer uso de una función, el algoritmo
principal la debe llamar. Por ejemplo:

```
real F(real X)
Inicio
    F = X /(1 + X ^2)
Fin
Inicio
   Imprimir "Este es el algoritmo principal"
   Leer N
   R = F(N)
   Imprimir "El resultado de la función es:",R
Fin
```

### Problemas Propuestos

1.  Diseñe un algoritmo que llene una matriz de `10 x 10` y determine:
    -   El numero mayor almacenado en la matriz
    -   El numero mayor almacenado en cada renglón
    -   La columna que tuvo la máxima suma
    -   El renglón que tuvo la máxima suma

    Diseña una función para cada inciso.
2.  Diseñe un algoritmo que lea un numero y mediante una función regrese el
    valor de 1 si el numero es positivo y -1 si es negativo.
