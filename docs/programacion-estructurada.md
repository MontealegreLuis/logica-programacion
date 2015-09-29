# Programación Estructurada

En este Capítulo se describe la historia de los lenguajes de programación, con
el fin de distinguir los diferentes paradigmas que existen, y así poder
introducir las características de la programación estructurada.

## Breve Historia de los Lenguajes de Programación

El comienzo de la historia de los lenguajes de programación data de mediados del
siglo XIX. Charles Babbage diseñó entre 1833 y 1842 la "máquina analítica", la
cual se considera como la primera computadora del mundo, pues pretendía realizar
cualquier tipo de cálculo. 

Desafortunadamente Babbage no pudo construirla por razones políticas y
financieras pero claro que era posible crear un programa que se ejecutara en
ella. En 1843 Babbage le pidió a Ada Augusta Byron King, condesa de Lovelace,
quien comprendía perfectamente el modelo de la máquina, que hiciera la
traducción al inglés de un documento escrito en francés que describía a la
máquina analítica. Ada Lovelace tardó más de un año en hacerlo, la traducción
incluía además unas notas en las que describía las instrucciones necesarias para
el funcionamiento de la máquina, es decir, un lenguaje de programación de
propósito general e incluso especificaba la forma de calcular los números de
Bernoulli usando tarjetas perforadas. Por esta razón se considera a Ada Lovelace
como la primera programadora teórica en la historia.

Años más tarde, gracias al trabajo desarrollado entre otros por John Presper
Eckert, John William Mauchly, Arthur Burks y finalemte por John von Neumann, la
arquitectura moderna de las computadoras sigue siendo la misma, salvo algunas
variaciones pero con el mismo principio: tener en la memoria tanto al programa
como a los datos sobre los que se opera.

Esta arquitectura, que lleva el nombre de von Neumann desde 1945, consta de
la unidad aritmético-lógica (ALU), la unidad de control, la memoria,
dispositivos de entrada/salida y el canal de datos.

Las primeras computadoras con esta arquitectura se tenían que programar a bajo
nivel, es decir, usando lenguaje de máquina. La programación era directamente
en binario; con secuencias de 0s y 1s que representaban datos e instrucciones
precisas para ser ejecutadas en la computadora en cuestión, la programación era
extremadamente compleja, si acaso se facilitó un poco al poder escribir el
programa en notación hexadecimal.

Sin embargo la idea de Grace Hopper de formar palabras llamadas opcodes (códigos
de operación) fue mejor ya que en realidad eran mnemónicos que se iban a
sustituir por instrucciones en lenguaje de máquina con ayuda de un compilador.
A ese compilador se le llamó ensamblador. En 1952 el equipo de Grace Hopper
desarrolló el lenguaje A-0 para la UNIVAC (UNIVersal Automatic Computer) en el
que se podían escribir expresiones aritméticas simples que se compilaban a
lenguaje de máquina ejecutable.

En 1954 John Backus desarrolló un lenguaje para la IBM 701 llamado Speedcoding
con características semejantes al A-0.

## Programación Estructurada

Las estructuras de control o estructuras algorítmicas son un grupo de formas de
trabajo, que permiten modificar el flujo de ejecución de las instrucciones de un
algoritmo o programa, con el fin de realizar ciertos procesos específicos que
nos lleven a la solución de problemas. El orden de ejecución de las sentencias o
instrucciones determinan el flujo de ejecución. Estas estructuras se clasifican
de acuerdo con su complejidad como se describe en la siguiente Figura:

![Tipos de estructuras](images/tipos-estructuras.png)

A la programación que utiliza estas estructuras se le conoce como **programación
estructurada**. La programación estructurada hace los programas más fáciles de
escribir, verificar, leer y mantener, ya que utilizan un número limitado de
estructuras de control que minimizan la complejidad de los problemas.

El término programación estructurada se refiere, a un conjunto de técnicas que
han ido evolucionando desde los primeros trabajos del holandés Edsger Dijkstra.
En mayo de 1996, Corrado Böhm y Giuseppe Jacopini demostraron que un **programa
propio** puede escribirse utilizando sólamente tres tipos de estructuras de
control: secuenciales, condicionales y cíclicas. A esto se le llama
**teorema de la programación estructurada**.

Un programa se define como propio si cumple lo siguiente:

-   Posee un sólo punto de inicio y uno de fin.
-   Existe al menos un camino desde el inicio hasta el fin que se puede seguir y
    que pasa por todas las partes del programa.
-   Todas las instrucciones son ejecutables y no existen lazos o ciclos infinitos.

## Paradigmas de Programación

Dependiendo de las técnicas y del lenguaje de programación que se elijan, se
puede hablar de "paradigmas de programación". Los principales son:

-   **Programación Estructurada**. Esta programación utiliza un número limitado
    de estructuras de control, reduciendo así considerablemente los errores.
    Esta técnica incorpora:
    -   Diseño descendente (**top-down**): el problema se descompone en etapas o
        estructuras jerárquicas que van de lo general a lo específico.
    -   Estructuras básicas: existen tres tipos de estructuras básicas:
        -   Estructuras secuenciales.
        -   Estructuras selectivas.
        -   Estructuras repetitivas.
    Un programa esta estructurado si posee un único punto de entrada y sólo uno
    de salida, existen de "1 a n" caminos desde el principio hasta el fin del
    programa.
-   **Programación modular**. La programación modular consta de varias secciones
    dividas de forma que interactúan a través de llamadas entre las secciones
    (procedimientos o funciones) que integran el programa en su totalidad. En la
    programación modular, el programa principal coordina las llamadas a los
    módulos secundarios y pasa los datos necesarios en forma de parámetros. A su
    vez cada módulo puede contener sus propios datos y llamar a otros módulos.
-   **Programación Orientada a Objetos**. El elemento principal de la
    programación orientada a objetos es el objeto. El objeto es un conjunto
    complejo de datos y programas que poseen estructura y un comportamiento
    definidos.
