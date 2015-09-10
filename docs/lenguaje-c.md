El lenguaje de programación C {#cap:LenguajeC}
=============================

EL lenguaje C es el resultado de un proceso de desarrollo que inició con
un lenguaje denominado BCPL escrito por Martin Richards. Este influenció
a otro llamado B (inventado por Ken Thompson). En los años 70’s para el
primer sistema UNIX en un DEC PDP-7; éste lenguaje llevó a la aparición
del C. El primer compilador de C fue escrito por Kernighan y Dennis
Ritchie en 1972 en la ATT para un DEC PDP-11 y escribió el propio
sistema operativo en C.

Con la popularidad de las microcomputadoras muchas compañías comenzaron
a implementar su propio C por lo cual surgieron discrepancias entre sí.
Por esta razón el ANSI (<span>*American National Standars
Institute*</span>), estableció un comité en 1983 para crear una
definición no ambigua del lenguaje C e independiente de la máquina que
pudiera utilizarse en todos los tipos de C. Algunos de las C existentes
son:

-   Ansi C

-   Zortech C++

-   Quick C

-   C++

-   Turbo C

-   Turbo C++

-   Borland C

-   Microsoft C

-   Visual C

-   C Builder

C es un lenguaje de programación de nivel medio ya que combina los
elementos del lenguaje de alto nivel con la funcionalidad del
ensamblador. Su característica principal es ser portable, es decir, es
posible adaptar los programas escritos para un tipo de computadora en
otra. Otra de sus características principales es el ser estructurado. El
lenguaje C inicialmente fue creado para la programación de:

-   Sistemas operativos

-   Intérpretes

-   Editores

-   Ensambladores

-   Compiladores

-   Administradores de bases de datos

Actualmente, debido a sus características, puede ser utilizado para todo
tipo de programas.

Traductores de programas
------------------------

Los traductores son programas que traducen los programas en código
fuente, escritos en lenguajes de alto nivel, a programas escritos en
lenguaje máquina. Los traductores pueden ser de dos tipos: compiladores
e interpretes

### Compiladores

Un <span>*compilador es un programa que traduce*</span> un programa
escrito en un lenguaje de programación, llamado <span>*lenguaje
fuente*</span>, a otro lenguaje de programación, llamado <span>*lenguaje
objeto*</span>, generando un programa equivalente que la máquina será
capaz de interpretar. Usualmente el segundo lenguaje es lenguaje de
máquina, pero también puede ser simplemente texto.

Además el compilador realiza una comprobación de errores en el programa,
es decir, revisa que todo este en orden por ejemplo <span>*variables e
instrucciones bien definidas*</span>, revisa todo lo referente a
<span>*cuestiones sintácticas*</span>. Está fuera del alcance del
compilador verificar que el algoritmo utilizado en el programa funcione
bien. A este proceso de traducción se le conoce como
<span>*compilación*</span>. La Figura [fig:procesoCompilacion] ilustra
el proceso de compilación aquí descrito.

De esta manera un programador puede diseñar un programa en un lenguaje
mucho más cercano a como piensa un ser humano, para luego compilarlo a
un programa manejable por una computadora.

Entrando en más detalle un programa se captura en un editor, el cual
produce un programa fuente, que a su vez es compilado obteniendo un
archivo parcial (<span>*un programa objeto*</span>) que tiene extensión
<span>.obj</span> luego el compilador invoca al montador
<span>*linker*</span> que convierte el programa objeto en un programa
ejecutable con extensión <span>.exe</span> que como ya sabemos es un
archivo que esta en formato binario (ceros y unos) y que puede funcionar
por sí solo. La Figura [fig:procesoEjecucion] muestra los pasos que se
suceden para obtener un programa ejecutable desde el código fuente:

### Intérpretes

Un intérprete es un programa capaz de <span>*analizar y ejecutar
programas escritos en un lenguaje de alto nivel*</span>. Los intérpretes
se diferencian de los compiladores en que mientras los compiladores
traducen un programa desde un lenguaje de programación a código máquina,
los primeros (los interpretes) sólo realizan la traducción a medida que
sea necesario, típicamente, <span>*instrucción por instrucción*</span>,
y normalmente no guardan el resultado de dicha traducción. La Figura
[fig:procesoInterprete] describe el proceso realizado por un intérprete.

Los programas interpretados suelen ser <span>*más lentos*</span> que los
compilados debido a la necesidad de traducir el programa mientras se
ejecuta, pero a cambio <span>*son más flexibles como entornos de
programación y depuración*</span> (lo que se traduce, por ejemplo, en
una mayor facilidad para reemplazar o agregar partes enteras a un
programa), y permiten ofrecer al programa interpretado un <span>*entorno
independiente de la máquina donde se ejecuta el intérprete*</span> (lo
que se conoce comúnmente como <span>*máquina virtual*</span>).

Comparando su actuación con la de un ser humano, <span>*un compilador
equivale a un traductor profesional*</span> que, a partir de un texto,
prepara otro independiente traducido a otra lengua, mientras que un
<span>*intérprete corresponde al intérprete humano*</span>, que traduce
de viva voz las palabras que oye, sin dejar constancia por escrito.

### Puesta a punto de un programa

La puesta a punto del programa hace referencia a la
<span>*localización*</span>, <span>*verificación*</span> y
<span>*corrección de errores de programación*</span> para obtener un
programa que funcione correctamente. La puesta a punto consta de las
siguientes etapas:

1.  <span>*Detección de errores*</span>. Esta etapa ocurre al compilar o
    ejecutar un programa. Sirve para verificar que el programa está bien
    escrito (al compilar) y que devuelve resultados correctos (al
    ejecutar).

2.  <span>*Depuración de errores*</span>. Esta fase consta de dos
    partes:

    -   <span>*Localización*</span>. Consiste en ubicar la(s) línea(s)
        de código que está(n) mal escrita(s) o que está(n) produciendo
        resultados incorrectos.

    -   <span>*Eliminación*</span>. Una vez ubicado el error se prosigue
        a corregirlo.

3.  <span>*Prueba del programa*</span>. Después de ubicar y corregir los
    errores se debe comprobar que los cambios fueron pertinentes. En
    caso de encontrar o producir nuevos errores se debe volver al paso
    1.

Los errores típicos que se presentan en un programa son:

-   Errores de sintaxis

-   Errores de lógica

#### Errores de sintaxis

Los errores de sintaxis se originan en el momento de
<span>*compilación/interpretación*</span> del programa y se deben a
<span>*causas propias de la sintaxis del lenguaje*</span> como
escrituras incorrectas de instrucciones, omisión de signos, etc. Estos
errores se descubren con <span>*facilidad*</span>.

#### Errores de lógica

Los errores en la lógica del programa pueden ser producidos en la fase
de <span>*compilación*</span> o <span>*ejecución*</span>. Los que
suceden durante la ejecución de un programa, normalmente, son más
<span>*difíciles de detectar*</span>. Se pueden observar dos categorías:
los que <span>*detienen la ejecución del programa*</span> y <span>*los
que no la detienen*</span>, pero que producen resultados erróneos.

-   Por ejemplo: si se tiene la asignación <span>r=s/c</span> y
    <span>c</span> es cero, se produce un error de <span>*división por
    cero*</span>. Muchos de los errores lógicos solo se manifiestan en
    el momento de la ejecución; por ello se denominan también errores de
    ejecución.

-   Un ejemplo más puede ocurrir con la asignación
    <span>l=2\*p\*r</span>. Si se omite el segundo símbolo del producto
    , la instrucción se convierte en <span>l=2\*pr</span>, la omisión de
    este símbolo no se reconoce como error de sintaxis en la fase de
    compilación o interpretación, pero daría resultados erróneos al
    ejecutarse.

Elementos básicos de un programa
--------------------------------

En el ámbito general, un programa codificado o escrito bajo cualquier
lenguaje de programación estructurado consta básicamente de dos
secciones:

-   Sección de encabezado

-   Sección de cuerpo de programa

#### La sección de encabezado

La sección de <span>*encabezado*</span> es usada para <span>*declarar
las variables y/o constantes*</span> (con sus respectivos
<span>*tipos*</span>) que se vayan a utilizar en el programa, así como
también el nombre de las funciones y/o procedimientos[^3] que ejecutarán
las instrucciones de los algoritmos que incluye dicho programa. Además
en esta sección se declaran los <span>*archivos de inclusión*</span>
(archivos generalmente con extensión <span>.h</span> hablando de
lenguaje C) que permiten el uso de algunas funciones que son necesarias
para el desarrollo del programa. Igualmente se especifican las
estructuras de datos complejas que se vayan a manejar.

#### La sección de cuerpo de programa

En la sección cuerpo de programa realmente se describen todos los
procedimientos y/o funciones que se van a ejecutar dentro del programa
así como también el código del <span>*programa principal*</span>. En un
cuerpo de programa es <span>*obligatorio*</span> que haya una
<span>*parte principal*</span> delimitada por <span>Begin …End</span>
para Pascal ó <span>void main() { …}</span> para lenguaje C) mientras
que los procedimientos y/o funciones son opcionales.

Elementos de un programa en C
-----------------------------

El siguiente ejemplo ilustra algunos de los componentes que con mayor
frecuencia se usan cuando se trata de codificar programas utilizando el
lenguaje de programación C.

     #include<stdio.h>

     /**
      * Programa que lee un numero ingresado por teclado
      * y lo muestra en pantalla
      */
     void main() {
        int numero;
        printf("Digite un numero entre 1 y 100");
        scanf("%d",&numero);
        printf("\n El numero que ingreso es: %d",numero);
     }

En las secciones siguientes se explican cada una de las partes de este
ejemplo.

### La directiva <span>\#include</span>

La directiva <span>\#include</span> da instrucciones al compilador C
para que añada el contenido de un <span>*archivo de inclusión*</span> al
programa durante la compilación. Un archivo de inclusión es un archivo
contiene información necesaria para el compilador. Varios de estos
archivos (algunas veces llamados archivos de encabezado) se proporcionan
con el compilador. <span>*Nunca*</span> se necesita modificar la
información de estos archivos y esta es la razón por la cual se
mantienen separados del código fuente. Todos los archivos de inclusión
deben tener la extensión (<span>.h</span>) por ejemplo
<span>\#include$<$stdio.h$>$</span>. En el caso del archivo de inclusión
<span>stdio.h</span> le indica al compilador que se han incluido
funciones estándares <span>std</span> de entrada <span>i=input</span> y
salida <span>o=output</span> que podrá utilizar en el desarrollo del
programa por ejemplo funciones como <span>printf()</span> y
<span>scanf()</span>.

La directiva <span>\#include</span>, en este programa de ejemplo,
significa “añada el contenido del archivo <span>stdio.h</span>”.

### La función <span>main</span>

La palabra <span>main</span> es muy importante y debe aparecer solo una
vez en todo programa C. En C, todo el código está basado en funciones.
El programa principal no es la excepción. <span>main()</span> indica el
comienzo de la función principal del programa la cual se <span>delimita
con llaves</span>. Este componente es obligatorio en cualquier programa
que se compile con lenguaje C. En su forma simple la función
<span>main</span> consiste en la palabra <span>void</span>, la cual
indica que la función <span>main</span> no devuelve ningún valor como
resultado, seguida de la palabra <span>main</span>, la cual representa
el nombre de la función, seguida de paréntesis <span>()</span> y las
instrucciones que ejecutan se encuentran demarcadas por las dos llaves
<span>{ </span> para indicar <span>Inicio</span> y <span>} </span> para
indicar <span>Fin</span>.

### Definición de identificadores

<span>*Un identificador es un nombre asignado a una posición de
almacenamiento de datos*</span> (variable o constante). El programa
utiliza variables para guardar varios tipos de datos durante la
ejecución del programa. En C, <span>*una variable debe definirse antes
de que pueda ser usada*</span>. Una definición de variable le informa al
compilador el nombre de la variable y el tipo de datos que va a guardar.
En el programa de ejemplo la definición de la línea <span>int
numero;</span> define una variables, llamadas <span>numero</span> que
guardará cada una un valor de tipo entero.

Las variables se pueden declarar en la zona de encabezado de un programa
o al inicio de una función o un procedimiento. Dos reglas se deben tener
en mente cuando se definen los identificadores son:

1.  El “tamaño” de los caracteres alfabéticos es importante. Usar
    <span>PRINCIPAL</span> para el nombre de una variable en C, no es lo
    mismo que usar <span>principal</span>, como tampoco es lo mismo que
    usar <span>PrInCiPaL</span>. Las tres palabras se refieren a
    variables o identificadores diferentes.

2.  De acuerdo al estándar ANSI-C, al darle nombre a un identificador
    solo serán significativos los primeros 31 caracteres, todo caracter
    mas allá de este límite será ignorado por cualquier compilador que
    cumpla la norma ANSI-C

Un elemento importante es el símbolo de subrayado <span>\_</span> que
puede utilizarse como parte del nombre de una variable. Debido a que una
gran parte de los escritores de compiladores utilizan el subrayado como
primer carácter para los nombres de variables internas de sistema, es
aconsejable evitar el uso del subrayado para iniciar un identificador y
así evitar la posibilidad de una confusión de nombres en la etapa de
compilación. Los identificadores con doble subrayado <span>\_\_</span>
están reservados para uso del compilador así como los identificadores
que empiezan con un subrayado seguido de una letra mayúscula, por
ejemplo <span>\_A</span>. Esto es importante, respetar ésta sencilla
regla evitará depurar errores innecesarios.

#### Tipos de datos en C

Para definir un identificador en C es necsario especificar su tipo de
dato. Los identificadores de tipos de datos, son un subconjunto de
identificadores que en cualquier lenguaje de programación se conocen
como <span>*palabras reservadas*</span>. Dichas palabras reservdas son
de uso exclusivo del compilador y no pueden usarse como identificadores
de variables y constantes. Los tipos de datos definidos en C son:

-   <span>int</span> Indica un tipo de dato entero con signo de 16, 32 ó
    64 bits, dependiendo del compilador. En sistemas de 16 bits su rango
    de valores es de -32768 a 32767. Para sistemas de 32 bits el rango
    es de -2147483648 a 2147483647. En sistemas de 64 bits el rango será
    de $1.7^{+/-308}$. Actualmente son muy pocos los compiladores con
    capacidad de manejar datos de tipo <span>int</span> de 64 bits, lo
    usual son sistemas de 16 ó 32 bits.

-   <span>float</span> Permite almacenar un número real de 32 bits cuyo
    rango va de $3.4^{+/-38}$. Generalmente su precisión es de 7
    dígitos.

-   <span>char</span> Un tipo de dato específico para manejo de
    caracteres de 8 bits de rango igual a -128 a 127.

Existen más tipos definidos en C pero por el momento solo será necesario
usar los tipos aquí descritos.

### La función <span>printf()</span>

La función <span>printf()</span> es una función de la biblioteca
<span>stdio.h</span> que despliega información en la pantalla. Acepta un
<span>*string de formato*</span> y cualquier número de argumentos. Estos
argumentos se aplican a cada uno de los <span>*especificadores de
formato*</span> contenidos en <span>format</span>. Un especificador de
formato toma la forma: %F, donde F indica el tipo de datos al que se
debe dar formato.

El tipo puede ser:

<span>%d</span>, para números enteros <span>%f</span> para números
reales y <span>%c</span> para caracteres

Por ejemplo,

     printf("Este es un mensaje simple");
     printf("Se muestra un numero entero %d", numeroEntero);
     printf("Se muestra un numero real %f", numeroReal);
     printf("Se muestra un numero entero %c", caracter);

### La función <span>scanf()</span>

La función <span>scanf()</span> es otra función de la librería o
biblioteca <span>stdio.h</span>. Ella lee datos desde el teclado y
asigna los datos a una o más variables del programa.

Por ejemplo: <span>scanf(“%d”,&a);</span> lee un valor entero y este es
asignado a la dirección de la variable <span>a</span>.

Estilo de Programación
----------------------

<span>*No basta con escribir un programa que funcione, el código tiene
que estar bien escrito*</span>. Muchas veces se escribe el código
pensando que la única persona que lo modificará es el mismo programador.
Y cuando llega alguien más, y comienza a revisar el código, comienzan
los problemas.

Que un programa funcione o no, es en buena medida <span>*independiente
de que esté bien o mal escrito*</span>. No obstante:

1.  Un programa mal escrito tiene una probabilidad mayor de no funcionar
    correctamente. Un buen estilo facilita la corrección.

2.  Es muy difícil depurar un programa mal escrito.

3.  Es muy costoso mantener un programa mal escrito.

Estos problemas se solucionan adoptando un <span>*estilo de
programación*</span>. El estilo de programación (también llamado
<span>*estándar de código*</span> o <span>*convención de código*</span>)
es un término que describe, en ciertos lenguajes de programación, un
acuerdo para escribir el código fuente de un programa con <span>*un
mismo formato*</span>.

Al igual que cuando aprendemos redacción literaria, una forma excelente
de adquirir un buen estilo es leer textos ajenos. Es por ello que se
recomienda la lectura, y el estudio, de programas existentes. Un
programa puede escribirse con mejor o peor estilo.

El buen estilo, al tratarse de algo subjetivo, es difícil de categorizar
concretamente; con todo, existen un número de <span>*características
generales*</span>. Con el advenimiento del software que da
<span>*formato al código fuente*</span> de forma automática, el foco en
cómo éste debe de ser escrito debe evolucionar de forma más amplia a la
<span>*elección de nombres*</span>, <span>*lógica*</span> y <span>*otras
técnicas*</span>.

Podemos clasificar los elementos a los que da formato el estilo de
programación de la siguiente forma:

Identificadores apropiados

:   Una pieza clave para un buen estilo es la elección apropiada de
    identificadores. Los identificadores pobremente nombrados dificultan
    la lectura del código fuente y su comprensión. Se recomienda que un
    identificador contenga al menos una palabra completa y que cuando
    más incluya tres.

Estilo de indentación

:   Indentación es un anglicismo de uso común en programación. Por
    indentación se entiende mover un bloque lógico de código hacia la
    derecha insertando espacios o tabuladores para separarlo de los
    delimitadores de bloques, (por ejemplo las llaves en C). La
    indentación es también un punto clave del buen estilo. Usando un
    estilo lógico y consistente hace que el código sea más legible.

En las siguientes secciones se detallará parte del estilo de
programación de Java, se ha elegido utilzarlo porque Java está basado en
C y por ser un lenguaje muy difundido que se sigue utilizando.

### Indentación

Se deben usar cuatro espacios como la unidad de indentación.

#### Tamaño de la línea

Se deben evitar las líneas mayores a 80 caracteres. El tamaño de las
líneas de documentación deben ser ligeramente menor al de las líneas de
código, no deben ser mayores a los 70 caracteres.

#### División de líneas

Cuando una expresión no quepa en una sola línea se debe dividir de
acuerdo a las siguientes reglas:

-   Divida después de una coma.

-   Divida antes de un operador.

-   Indente la línea nueva al inicio de la expresión al mismo nivel que
    la línea anterior.

-   Si las reglas anteriores producen código confuso que se encuentre
    muy a la derecha, indente sólo con 8 espacios.

Oberve los siguientes ejemplos:

    nombreLargo1 = nombreLargo2 * nombreLargo3 + nombreLargo4
                   + 4 * nombreLargo5

    printf("Ejemplo de linea larga dividida en %d partes",
            variasPartes);

### Comentarios

Los comentarios forman parte de la documentaci’on interna de un
programa. Se distinguen dos tipos de comentarios: <span>*comentarios de
implementación*</span> y <span>*comentarios de documentación*</span>.
Los comentarios de implementación son aquellos que están delimitados por
<span>/\*...\*/</span> y <span>//</span>. Los comentarios de
documentación están delimitados por <span>/\*\*...\*/</span> y son
nativos de Java.

Comentarios de implementación

:   Los comentarios de implementación son un medio para comentar código
    y explicar los <span>*detalles de la implementación*</span>.

Comentarios de documentación

:   Los comentarios de documentación están diseñados para
    <span>*describir la especificación del código*</span> sin tomar en
    cuenta la implementación. Están dirigidos a desarrolladores que
    podrían no contar con el código fuente.

Los comentarios se deben usar para dar describir brevemente código y
proporcionar información adicional que no se encuentra disponible de
manera obvia en el código. Los comentarios sólo deben tener información
relevante para la <span>*comprensión del programa*</span>.

<span>**Nota**</span>: La frecuencia de los comentarios refleja con
frecuencia código de mala calidad. Cuando se sienta la necesidad de
agregar un comentario, se debe considerar la posibilidad de reescribir
el código a fin de hacerlo más claro.

#### Comentarios de implementación

Los programas pueden tener cuatro tipos de comentarios de
implementación: <span>*de bloque*</span>, <span>*de una sola
línea*</span>, <span>*de seguimiento*</span> y <span>*de fin de
línea*</span>.

##### Comentarios de bloque

Los comentarios de bloque se usan para proporcionar descripciones de
<span>*programas*</span>, <span>*funciones*</span>, <span>*estructuras
de datos*</span> y <span>*algoritmos*</span>. Estos comentarios deben
aparecer al inicio de un archivo fuente y antes de cada función.

También pueden usarse en otros lugares, por ejemplo adentro de las
funciones. Los comentarios de bloque dentro de una función deben
indentarse al mismo nivel del código que describen. Este tipo de
comentarios deben iniciarse con una línea en blanco para separarlos del
resto del código. Estos comentarios inician cada línea con un asterisco

     /*
      * Este es un comentario de bloque
      * que ocupa mas de una linea
      */

##### Comentarios de una línea

Se pueden escribir comentarios cortos en una sóla línea indentada al
mismo nivel que el código que se comenta. Si un comentario no se puede
escribir en una sola línea, se debe seguir el formato de bloque. Un
comentario de una línea debe estar precedido por una línea en blanco.

     /* Este es un comentario de una sola linea */

##### Comentarios de seguimiento

Algunos comentarios <span>*muy pequeños*</span> pueden aparecer en la
misma línea que el código que describen, pero deben separarse lo
suficiente para distinguirlos del código. Si hay más de un comentario
corto dentro del mismo bloque, todos deben indentarse a la misma altura.
Se debe evitar comentar cada línea de código.

     area=lado*lado;    /* Se calcula el area del cuadrado */

##### Comentarios de fin de línea

El delimitador de comentario <span>//</span> inicia un comentario de una
línea completa o un comentario de fin de línea. Puede comentar una línea
completa de código o sólo parte de la línea. No debe usarse en varias
líneas consecutivas.

     suma=a+b    // Se realiza la suma
     // Se muestra el resultado en pantalla
     printf("Es resultado de la suma es: %d",suma);

#### Comentarios de documentación

Los comentarios de documentación describen funciones. Cada comentario se
coloca dentro de los delimitadores <span>/\*\* …/</span>. Este
comentario debe aparecer antes de la declaración de una función. En el
siguiente ejemplo aparece antes de la función <span>main()</span>.

     /**
      * Este programa resuelve el siguiente problema: ...
      */
     void main() {
         ...
     }

Los comentarios de documentación no deben colocarse dentro de una
función.

##### Etiquetas de documentacion

Las etiquetas de documentación proporcionan información adicional sobre
una función o programa. Estas etiquetas inician con una arroba
<span>@</span>. Por el momento solo usaremos dos etiquetas:

@author

:   Esta eiqueta debe ir seguida por el nombre del autor del programa,
    con el formato <span>nombre(s) apellido(s)</span>.

@version

:   Esta etiqueta contiene la versión del programa, seguido de la fecha
    de creación con el formato <span>dd Mes aaaa</span>.

El siguiente es un comentario de documentación que utiliza las etiquetas
que se acaban de explicar.

     /**
      * Este programa resuelve el siguiente problema:
      * ...
      *
      * @author Luis Montealegre
      * @version 1.0 17 Sep 2008
      */
     void main() {
         ...
     }

### Declaraciones

A continuación se describen las reglas que se deben seguir al declarar
variables. Se revisarán aspectos tales como: dónde declarar e
inicializar variables.

#### Declaración por línea

Se recomienda una declaración por línea dado que fomenta la inclusión de
comentarios. Por ejemplo:

       int nivel;   // Almacena el nivel de indentacion
       int tamano;  // Tamano de la tabla

No se deben colocar tipos distintos en la misma línea, por ejemplo:

     int edad; float promedio;

#### Ubicación

Coloque las declaraciones solo al inicio de bloques de código. Un bloque
de código es cualquier conjunto de instrucciones rodeadas de “llaves”
<span>{</span> y <span>}</span>. No espere a declarar las variables
hasta antes de usarlas esto puede confundir a otros programadores,
observe el siguiente ejemplo:

     void main() {
         int edad; // inicio del bloque de la funcion main

         ...       // el resto de las instrucciones
     }

#### Inicialización

Trate de inicializar las variables locales donde se declaran. La única
razón para no hacerlo es que el valor inicial de la variable dependa del
resultado de alguna operación posterior a la declaración. Por ejemplo;

     void main() {
         int edad = 0; // se declara e inicializa "edad"

         ...       // el resto de las instrucciones
     }

### Espacio en blanco

En esta sección se describen las reglas para colocar líneas y espacios
en blanco dentro del código;

#### Líneas en blanco

Las líneas en blanco mejoran la legibilidad del código, separando las
secciones de código que están relacionadas lógicamente.

Se debe dejar una línea en blanco bajo las siguientes circunstancias:

-   Entre funciones.

-   Entre la declaración de variables en una función y la primera línea
    de código.

-   Antes de un comentario de bloque o de una sola línea

#### Espacios en blanco

Se debe colocar un espacio en blanco en las siguientes circunstancias:

-   Se debe colocar un espacio en blanco despues de una coma.

-   Todos los operadores binarios deben separarse de sus operadores.

### Ejemplo de programa completo

Los programas escritos en C, hasta ahora, deben seguir el siguiente
orden:

1.  Directivas para agregar archivos de inclusion.

2.  Comentario de documentación para la función <span>main</span>.

3.  La función <span>main</span>, la cual se puede dividir en las
    siguientes secciones:

    -   <span>*Declaración e inicializaci’on de variables*</span>, cada
        variable debe ir seguida de un comentario de
        <span>*seguimiento*</span> que explique la función y/o
        significado de la variable dentro del programa.

    -   <span>*Grupo de instrucciones de lectura de variables de
        entrada*</span>, antecedidas de un comentario de una sola línea
        o de bloque, que indique que variables se van a leer.

    -   <span>*Grupo de instrucciones de proceso*</span>, las cuales
        deben explicarse usando un comentario de una sola línea o de
        bloque.

    -   <span>*Grupo de instrucciones de salida en pantalla*</span>, las
        cuales se comentan del mismo modo que los dos grupos de
        instrucciones descritos anteriormente.

Observe el siguiente ejemplo, note que incluye cada una de las partes
mencionadas con anterioridad.

     #include<stdio.h>
     #include<conio.h>

     /**
      * Este programa resuelve el siguiente problema:
      * Escriba un programa que calcule el area de un
      * rectangulo
      *
      * @author Luis Montealegre
      * @version 1.0 17 Sep 2008
      */
     void main() {
         float base;   /* El valor de la base en metros */
         float altura; /* El valor de la altura en metros */
         float area;   /* El valor del area en metros */

         clrscr();

         /* Se leen los valores de la base y la altura */
         printf("Ingrese el valor de la base:");
         scanf("%f", &base);
         printf("Ingrese el valor de la altura:");
         scanf("%f", &altura);

         /* Se calcula el area */
         area = base * altura;

         /* Se muestra el valor del area */
         printf("El area es de %d metros", area);

         getch();
     }
