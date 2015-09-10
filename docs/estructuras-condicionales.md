Estructuras Condicionales 
=========================

Las estructuras condicionales comparan una variable contra otro(s)
valor(es), para que en base al resultado de esta comparación, se siga un
curso de acción dentro del programa. Cabe mencionar que la comparación
se puede hacer contra otra variable o contra una constante, según se
necesite. Existen dos tipos básicos, las simples y las múltiples.

Estructuras Condicionales Simples
---------------------------------

Dentro del grupo de estructuras simples existe una subdivisón que
implica dos tipos de condicionales las <span>*sencillas*</span> y las
<span>*dobles*</span>.

### Condicionales Sencillas

Las estructuras condicionales sencillas se les conoce como ”Tomas de
decisión”. Estas tomas de decisión tienen la siguiente forma:

        si <condicion> entonces
        inicio-si
            <acciones-si>
        fin-si

#### Condicionales Dobles

Las estructuras condicionales dobles permiten elegir entre dos opciones
o alternativas posibles en función del cumplimiento o no de una
determinada condición. Se representan de la siguiente forma:

        si <condicion> entonces
        inicio-si
            <acciones-si>
        fin-si
        si no
        inicio-si no
            <acciones-si no>
        fin-si no

Donde:

-   <span>si</span>. Indica el comando de comparación

-   <span>condicion</span>. Indica la condición a evaluar

-   <span>entonces</span>. Precede a las acciones a realizar cuando se
    cumple la condición.

-   <span>acciones-si</span>. Son las acciones a realizar cuando se
    cumple la condición.

-   <span>si no</span>. Precede a las acciones a realizar cuando no se
    cumple la condición.

-   <span>acciones-si-no</span>. Son las acciones a realizar cuando no
    se cumple la condición.

Dependiendo de si la comparación es cierta o falsa, se pueden realizar
una o más acciones.

### Problemas Selectivos Simples

1.  Un hombre desea saber cuanto dinero se genera por concepto de
    intereses sobre la cantidad que tiene en inversión en el banco. El
    decidirá reinvertir los intereses siempre y cuando estos excedan a
    \$7000, y en ese caso desea saber cuanto dinero tendrá finalmente en
    su cuenta. Suponga que el interés que cobra el banco es un dato
    desconocido.

        inicio
         escribir "Que porcentaje de intereses cobra tu banco?"
         leer porcentajeInteres
         escribir "Cuanto vas a invertir?"
         leer capital
         intereses = capital * porcentajeIntereses / 100
         si intereses > 7000 entonces
         inicio-si
            inversion = capital +intereses
         fin-si
         escribir "Al final tu capital sera de ", inversion
        fin

2.  Determinar si un alumno aprueba a reprueba un curso, sabiendo que
    aprobara si su promedio de tres calificaciones es mayor o igual a
    70; reprueba en caso contrario.

        inicio
          escribir "Cual es tu primer calificacion?"
          leer calificacionUno
          escribir "Cual es tu segunda calificacion?"
          leer calificacionDos
          escribir "Cual es tu tercer calificacion?"
          leer calificacionTres
          promedio =
           (calificacionUno+calificacionDos+calificacionTres)/3
          si promedio >= 70 entonces
          inicio-si
            escribir "Felicidades aprobaste..."
          fin-si
          si no
          inicio-si no
            escribir "Lo siento, reprobaste..."
          fin-si no
        fin

3.  En un almacén se hace un 20% de descuento a los clientes cuya compra
    supere los \$1000 ¿ Cual será la cantidad que pagara una persona por
    su compra?

            inicio
               escribir "Cuanto compraste?"
               leer compra
               si compra > 1000 entonces
               inicio-si
                 descuento = compra * 0.20
               fin-si
               si no
               inicio-si no
                 desc = 0
               fin-si no
               total = compra - descuento
               escribir "Vas a pagar", total
            fin

4.  Hacer un algoritmo que calcule el total a pagar por la compra de
    camisas. Si se compran tres camisas o mas se aplica un descuento del
    20% sobre el total de la compra y si son menos de tres camisas un
    descuento del 10%

            inicio
               escribir "Cuanto cuesta cada camisa?"
               leer precio
               escribir "Cuantas camisas compraste?"
               leer numeroCamisas
               compra = numeroCamisas * precio
               si numeroCamisas > = 3 entonces
               inicio-si
                 total = compra - compra * 0.20
               fin-si
               si no
               inicio-si no
                 total = compra - compra * 0.10
               fin-si no
               escribir "Vas a pagar ", total
            fin

5.  Escriba un algoritmo que lea dos números y los imprima en forma
    ascendente

            inicio
               escribir "Dame un numero"
               leer numeroUno
               escribir "Dame otro numero"
               leer numeroDos
               si numeroUno < numeroDos entonces
               inicio-si
                 escribir "1.-",numeroUno," 2.-",numeroDos
               fin-si
               si no
               inicio-si no
                 Escribir "1.-",numeroDos," 2.-",numeroUno
               fin-si no
            fin

6.  Un obrero necesita calcular su salario semanal, el cual se obtiene
    de la siguiente manera:

    -   Si trabaja 40 horas o menos se le paga \$16 por hora

    -   Si trabaja mas de 40 horas se le paga \$16 por cada una de las
        primeras 40 horas y \$20 por cada hora extra.

    <!-- -->

            inicio
               escribir "Cuantas horas trabajaste?"
               leer horasTrabajadas
               si horasTrabajadas > 40 entonces
               inicio-si
                    horasExtras = horasTrabajadas - 40
                    salarioSemanal = horasExtras * 20 + 40 * 16
               fin-si
               si no
               inicio-si no
                    salarioSemanal = horasTrbajadas * 16
               fin-si no
               escribir "Vas a cobrar: ", salarioSemanal
            fin

7.  Una persona enferma, que pesa 70 Kg., se encuentra en reposo y desea
    saber cuantas calorías consume su cuerpo durante todo el tiempo que
    realiza una misma actividad. Las actividades que tiene permitido
    realizar son únicamente dormir o estar sentado en reposo. Los datos
    que tiene son que estando dormido consume 1.08 calorías por minuto y
    estando sentado en reposo consume 1.66 calorías por minuto.

            inicio
               esribir "Que actividad estas realizando?"
               leer actividad
               escribir "Cuanto tiempo llevas asi?"
               leer tiempo
               si actividad == 'd' entonces
               inicio-si
                  calorias = 1.08 * tiempo
               fin-si
               si no
               inicio- si no
                  calorias = 1.66 * tiempo
               fin-si no
               escribir "Consumes", calorias, " calorias"
            fin

8.  Hacer un algoritmo que imprima precio original y el precio con
    descuento de un artículo. El descuento lo hace en base a la clave,
    si la clave es 1 el descuento es del 10% y si la clave es 2 el
    descuento en del 20% (solo existen dos claves).

        inicio
         escribir "Cual es el precio original del articulo?"
         leer precioOriginal
         escribir "Cual es la clave del articulo?"
         leer claveArticulo
         si claveArticulo == 1 entonces
         inicio-si
           precioDescuento=precioOriginal-precioOriginal*0.10
         fin-Si
         si no
         inicio-si no
           precioDescuento=precioOriginal-precioOriginal*0.20
         fin-si no
         escribir "El precio original es de: ",precioOriginal
         escribir "Ya con el descuento es de: ",precioDescuento
        fin

9.  Una empresa quiere hacer una compra de varias piezas de la misma
    clase a una fábrica de refacciones. La empresa, dependiendo del
    monto total de la compra, decidirá que hacer para pagar al
    fabricante.

    Si el monto total de la compra excede de \$500 000 la empresa tendrá
    la capacidad de invertir de su propio dinero un 55% del monto de la
    compra, pedir prestado al banco un 30% y el resto lo pagara
    solicitando un crédito al fabricante. Si el monto total de la compra
    no excede de \$500 000 la empresa tendrá la capacidad de invertir de
    su propio dinero un 70% y el restante 30% lo pagara solicitando
    crédito al fabricante. El fabricante cobra por concepto de intereses
    un 20% sobre la cantidad que se le pague a crédito.

        inicio
            escribir "Cuanto cuesta cada pieza?
            leer costoPieza
            escribir "Cuantas ´piezas compraste?"
            leer numeroPiezas
            total = costopieza * numeroPiezas
            si total > 500 000 entonces
            inicio-si
                cantidadInvertida = total * 0.55
                prestamo = total * 0.30
                credito = total * 0.15
            fin-si
            si no
            inicio-si no
                cantidadInvertida= total * 0.70
                credito = total * 0.30
                prestamo = 0
            fin - si no
            intereses = credito * 0.20
            escribir "Invertiste ", intereses
            escribir "Vas a pedir prestado ", prestamo
            escribir "De credito es ",credito
            escribir "De intereses es", intereses
        fin

### Problemas Propuestos

1.  Leer un número y escribir el valor absoluto del mismo.

2.  Calcular el total que una persona debe pagar en un llantera, si el
    precio de cada llanta es de \$800 si se compran menos de 5 llantas y
    de \$700 si se compran 5 o más.

3.  En un supermercado se hace una promoción, mediante la cual el
    cliente obtiene un descuento dependiendo de un número que se escoge
    al azar. Si el número escogido es menor que 74 el descuento es del
    15% sobre el total de la compra, si es mayor o igual a 74 el
    descuento es del 20%. Obtener cuanto dinero se le descuenta.

4.  Calcular el numero de pulsaciones que debe tener una persona por
    cada 10 segundos de ejercicio aeróbico; la fórmula que se aplica
    cuando el sexo es femenino es:

    <span>numeroPulsaciones = (220 - edad) / 10</span>

    y si el sexo es masculino:

    <span>numeroPulsaciones = (210 - edad) / 10</span>

5.  Una compañía de seguros esta abriendo un departamento de finanzas y
    estableció un programa para captar clientes, que consiste en lo
    siguiente: Si el monto por el que se efectúa la fianza es menor que
    \$50 000 la cuota a pagar será por el 3% del monto, y si el monto es
    mayor que \$50 000 la cuota a pagar será el 2% del monto. La
    afianzadora desea determinar cual será la cuota que debe pagar un
    cliente.

6.  En una escuela la colegiatura de los alumnos se determina según el
    número de materias que cursan. El costo de todas las materias es el
    mismo. Se ha establecido un programa para estimular a los alumnos,
    el cual consiste en lo siguiente: si el promedio obtenido por un
    alumno en el último periodo es mayor o igual que 9, se le hará un
    descuento del 30% sobre la colegiatura y no se le cobrará IVA; si el
    promedio obtenido es menor que 9 deberá pagar la colegiatura
    completa, la cual incluye el 10% de IVA. Obtener cuanto debe pagar
    un alumno.

7.  Una empresa de bienes raíces ofrece casas de interés social, bajo
    las siguientes condiciones: Si los ingresos del comprador son
    menores a \$8000 el enganche será del 15% del costo de la casa y el
    resto se distribuirá en pagos mensuales, a pagar en diez años. Si
    los ingresos del comprador son más de \$8000 el enganche será del
    30% del costo de la casa y el resto se distribuirá en pagos
    mensuales a pagar en 7 años. La empresa quiere obtener cuanto debe
    pagar un comprador por concepto de enganche y cuanto por cada pago
    parcial.

8.  El gobierno ha establecido el programa SAR (Sistema de Ahorro para
    el Retiro) que consiste en que los dueños de la empresa deben
    obligatoriamente depositar en una cuenta bancaria un porcentaje del
    salario de los trabajadores; adicionalmente los trabajadores pueden
    solicitar a la empresa que deposite directamente una cuota fija o un
    porcentaje de su salario en la cuenta del SAR, la cual le será
    descontada de su pago. Un trabajador que ha decidido aportar a su
    cuenta del SAR desea saber la cantidad total de dinero que estará
    depositado a esa cuenta cada mes, y el pago mensual que recibirá.

9.  Una persona desea iniciar un negocio, para lo cual piensa verificar
    cuanto dinero le prestará el banco por hipotecar su casa. Tiene una
    cuenta bancaria, pero no quiere disponer de ella a menos que el
    monto por hipotecar su casa sea muy pequeño. Si el monto de la
    hipoteca es menor que \$1 000 000 entonces invertirá el 50% de la
    inversión total y un socio invertirá el otro 50%. Si el monto de la
    hipoteca es de \$1 000 000 o más, entonces invertirá el monto total
    de la hipoteca y el resto del dinero que se necesite para cubrir la
    inversión total se repartirá a partes iguales entre el socio y él.

10. El gobierno del estado de México desea reforestar un bosque que mide
    determinado número de hectáreas. Si la superficie del terreno excede
    a 1 millón de metros cuadrados, entonces decidirá sembrar de la sig.
    manera:

    Si la superficie del terreno es menor o igual a un millón de metros
    cuadrados, entonces decidirá sembrar de la sig. manera:

    El gobierno desea saber el número de pinos, oyameles y cedros que
    tendrá que sembrar en el bosque, si se sabe que en 10 metros
    cuadrados caben 8 pinos, en 15 metros cuadrados caben 15 oyameles y
    en 18 metros cuadrados caben 10 cedros. También se sabe que una
    hectárea equivale a 10 mil metros cuadrados.

11. Una fabrica ha sido sometida a un programa de control de
    contaminación para lo cual se efectúa una revisión de los puntos
    IMECA generados por la fábrica. El programa de control de
    contaminación consiste en medir los puntos IMECA que emite la
    fábrica en cinco días de una semana y si el promedio es superior a
    los 170 puntos entonces tendrá la sanción de parar su producción por
    una semana y una multa del 50% de las ganancias diarias cuando no se
    detiene la producción. Si el promedio obtenido de puntos IMECA es de
    170 o menor entonces no tendrá ni sanción ni multa. El dueño de la
    fabrica desea saber cuanto dinero perderá después de ser sometido a
    la revisión.

12. Una persona se encuentra con un problema de comprar un automóvil o
    un terreno, los cuales cuestan exactamente lo mismo. Sabe que
    mientras el automóvil se devalúa, con el terreno sucede lo
    contrario. Esta persona comprara el automóvil si al cabo de tres
    años la devaluación de este no es mayor que la mitad del incremento
    del valor del terreno. Ayúdale a esta persona a determinar si debe o
    no comprar el automóvil.

Condicionales Múltiples
-----------------------

Las estructuras de comparación múltiples, son tomas de decisión
especializadas que permiten comparar una variable contra distintos
posibles resultados, ejecutando para cada caso una serie de
instrucciones especificas. La forma común es la siguiente:

        Si <condicion1> entonces
        Inicio-si
            Acciones1
        Fin-si
        si no
            Si <condicion2> entonces
            Inicio-si
                Acciones2
            Fin-si
            si no
                .
                .
                .

### Problemas Selectivos Compuestos

1.  Leer 2 números; si son iguales que los multiplique, si el primero es
    mayor que el segundo que los reste y si no que los sume.

        Inicio
            Escribir "Dame el primer numero:"
            Leer numeroUno
            Escribir "Dame el segundo numero:"
            Leer numeroDos
            si numeroUno == numeroDos entonces
            Inicio-si
                resultado = numeroUno * numeroDos
            Fin-si
            si no
            Inicio-Si no
                si numeroUno > numeroDos entonces
                Inicio-si
                    resultado = numeroUno - numeroDos
                Fin-si
                si no
                Inicio-si no
                    resultado = numeroUno + numeroDos
                Fin-si no
            Fin-si no
        Fin

2.  Leer tres números diferentes e imprimir el número mayor de los tres.

        Inicio
            Escribir "Dame el primer numero"
            Leer numeroUno
            Escribir "Dame el segundo numero"
            Leer numeroDos
            Escribir "Dame el tercer numero"
            Leer numeroTres
            Si (numeroUno > numeroDos) &&
               (numeroUno > numeroTres) entonces
                mayor = numeroUno
            si no
                Si (numeroDos > numeroUno) &&
                   (numeroDos > numeroTres) entonces
                    mayor = numeroDos
                si no
                    mayor = numeroTres
                fin-si
            fin-si
            Escribir "El mayor de los tres numeros es ",mayor
        fin

3.  Determinar la cantidad de dinero que recibirá un trabajador por
    concepto de las horas extras trabajadas en una empresa, sabiendo que
    cuando las horas de trabajo exceden de 40, el resto se consideran
    horas extras y que estas se pagan al doble de una hora normal cuando
    no exceden de 8; si las horas extras exceden de 8 se pagan las
    primeras 8 al doble de lo que se pagan las horas normales y el resto
    al triple.

        Inicio
            Escribir "Cuantas horas trabajaste?"
            Leer horasTrabajadas
            Escribir "Cual es el pago por hora?"
            Leer pagoHora
            pagoExtra=0
            Si horasTrabajadas < = 40 entonces
            Inicio-si
                pagoSimple = horasTrabajadas * pagoHora
            Fin-si
            si no
            Inicio-si no
                pagoSimple=40*pagoHora
                horasExtras = horasTrabajadas - 40
                Si horasExtras < = 8 entonces
                Inicio-si
                    pagoExtra = horasExtras * pagoHora * 2
                Fin-si
                si no
                Inicio-si no
                    pagoDoble = 8 * pagoHora * 2
                    pagoTriple=(horasExtras-8)*pagoHora*3
                    pagoExtra = pagoDoble + pagoTriple
                Fin-si no
            fin-si no
            total = pagoSimple + pagoExtra
            Escribir "Vas a ganar", total
        fin

4.  Calcular la utilidad que un trabajador recibe en el reparto anual de
    utilidades si éste se le asigna como un porcentaje de su salario
    mensual que depende de su antigüedad en la empresa de acuerdo con la
    siguiente tabla:

        Inicio
            Escribir "Cuanto ganas al mes?"
            Leer salarioMensual
            Escribir "Cual es tu antiguedad?"
            Leer antiguedad
            Si antiguedad < 1 entonces
            Inicio-si
                utilidad = salarioMensual * 0.05
            Fin-si
            si no
            Inicio-si no
                Si antiguedad < 2 entonces
                Inicio-si
                    utilidad = salarioMensual * 0.07
                Fin-si
                si no
                Inicio-si no
                    Si antiguedad < 5 entonces
                    Inicio-si
                        utilidad = salarioMensual * 0.10
                    Fin-si
                    si no
                    Inicio-si no
                        Si antiguedad < 10 entonces
                        Inicio-si
                            utilidad = salarioMensual * 0.15
                        Fin-si
                        si no
                        Inicio-si no
                            utilidad = salarioMensual * 0.20
                        Fin-si no
                    Fin-si no
                Fin-si no
            Fin-si no
            Escribir "Tu utilidad sera de ", utilidad
        Fin

5.  En una tienda de descuento se efectúa una promoción en la cual se
    hace un descuento sobre el valor de la compra total según el color
    de la bolita que el cliente saque al pagar en caja. Si la bolita es
    de color blanco no se le hará descuento alguno, si es verde se le
    hará un 10% de descuento, si es amarilla un 25%, si es azul un 50% y
    si es roja un 100%. Determinar la cantidad final que el cliente
    deberá pagar por su compra. se sabe que solo hay bolitas de los
    colores mencionados.

        Inicio
            Escribir "Cuanto compraste"
            Leer compra
            Escribir "De que color es la bolita?"
            Leer colorBolita
            si colorBolita = 'b' entonces
            Inicio-si
                descuento =0
            Fin-si
            si no
            Inicio-si no
                si colorBolita  = 'v' entonces
                Inicio-si
                    descuento =compra *0.10
                Fin-si
                si no
                Inicio-si no
                    si colorBolita  = 'a' entonces
                    Inicio-si
                        descuento =compra *0.25
                    Fin-si
                    si no
                    Inicio-si no
                        si colorBolita = 'z' entonces
                        Inicio-si
                            descuento = compra *0.50
                        Fin-si
                        si no
                        Inicio-si no
                            descuento=compra
                        fin-si no
                    fin-si no
                fin-si no
            fin-si no
            total=compra-descuento
            Escribir "Vas a pagar ", total
        Fin

6.  El IMSS requiere clasificar a las personas que se jubilarán en el
    año de 1997. Existen tres tipos de jubilaciones: por edad, por
    antigüedad joven y por antigüedad adulta. Las personas adscritas a
    la jubilación por edad deben tener 60 años o mas y una antigüedad en
    su empleo de menos de 25 años. Las personas adscritas a la
    jubilación por antigüedad joven deben tener menos de 60 años y una
    antigüedad en su empleo de 25 años o más. Las personas adscritas a
    la jubilación por antigüedad adulta deben tener 60 años o mas y una
    antigüedad en su empleo de 25 años o más. Determinar en que tipo de
    jubilación, quedará adscrita una persona.

        Inicio
          Escribir "Cual es tu edad?"
          Leer edad
          Escribir "Cual es tu antiguedad"
          Leer antiguedad
          si edad >= 60 && antiguedad < 25 entonces
          Inicio-si
             Escribir "Jubilacion por edad"
          Fin-si
          si no
          Inicio-si no
             si edad >= 60 && antiguedad > 25 entonces
             Inicio-si
                 Escribir "Jubilacion por edad adulta"
             Fin-si
             si no
             Inicio-si no
                 si edad < 60 && antiguedad > 25 entonces
                 Inicio-si
                    Escribir "Jubilacion por antiguedad joven"
                 Fin-si
                 si no
                 Inicio-si no
                    Escribir "no tiene porque jubilarse"
                 Fin-si no
            Fin-si no
          Fin-si
        Fin

### Problemas Propuestos

1.  En una fábrica de computadoras se planea ofrecer a los clientes un
    descuento que dependerá del número de computadoras que compre. Si
    las computadoras son menos de cinco se les dará un 10% de descuento
    sobre el total de la compra; si el número de computadoras es mayor o
    igual a cinco pero menos de diez se le otorga un 20% de descuento; y
    si son 10 o más se les da un 40% de descuento. El precio de cada
    computadora es de \$11,000

2.  En una llantera se ha establecido una promoción de las llantas marca
    “Ponchadas”, dicha promoción consiste en lo siguiente: si se compran
    menos de cinco llantas el precio es de \$300 cada una, de \$250 si
    se compran de cinco a 10 y de \$200 si se compran más de 10. Obtener
    la cantidad de dinero que una persona tiene que pagar por cada una
    de las llantas que compra y la que tiene que pagar por el total de
    la compra.

3.  En un juego de preguntas a las que se responde “Si” o “No” gana
    quien responda correctamente las tres preguntas. Si se responde mal
    a cualquiera de ellas ya no se pregunta la siguiente y termina el
    juego. Las preguntas son:

    1.  ?\`Colón descubrió América?

    2.  ?\`La independencia de México fue en el año 1810?

    3.  ?\`The Doors fue un grupo de rock Americano?

4.  Un proveedor de estéreos ofrece un descuento del 10% sobre el precio
    sin IVA, de algún aparato si este cuesta \$2000 o mas. Además,
    independientemente de esto, ofrece un 5% de descuento si la marca es
    “SONY”. Determinar cuanto pagara, con IVA incluido, un cliente
    cualquiera por la compra de su aparato.

5.  Una frutería ofrece las manzanas con descuento según la siguiente
    tabla:

    Determinar cuanto pagará una persona que compre manzanas en esa
    frutería.

6.  El dueño de una empresa desea planificar las decisiones financieras
    que se tomarán en el siguiente año. La forma de planificar depende
    de lo siguiente: si actualmente su capital se encuentra con saldo
    negativo, pedirá un préstamo bancario para que su nuevo saldo sea de
    \$10 000. Si su capital tiene actualmente un saldo positivo pedirá
    un préstamo bancario para tener un nuevo saldo de \$20 000, pero si
    su capital tiene actualmente un saldo superior a los \$20 000 no
    pedirá ningún préstamo. Posteriormente repartirá su presupuesto de
    la siguiente manera: \$5 000 para equipo de cómputo \$2 000 para
    mobiliario y el resto la mitad será para la compra de insumos y la
    otra para otorgar incentivos al personal. Desplegar que cantidades
    se destinaran para la compra de insumos e incentivos al personal y,
    en caso de que fuera necesario, a cuanto ascendería la cantidad que
    se pediría al banco.

7.  Tomando como base los resultados obtenidos en un laboratorio de
    análisis clínicos, un medico determina si una persona tiene anemia o
    no, lo cual depende de su nivel de hemoglobina en la sangre, de su
    edad y de su sexo. Si el nivel de hemoglobina que tiene una persona
    es menor que el rango que le corresponde, se determina su resultado
    como positivo y en caso contrario como negativo. La tabla en la que
    el medico se basa para obtener el resultado es la siguiente:

8.  Una institución educativa estableció un programa para estimular a
    los alumnos con buen rendimiento académico y que consiste en lo
    siguiente: Si el promedio es de 9.5 o mas y el alumno es de
    preparatoria, entonces este podrá cursar 55 unidades y se le hará un
    25% de descuento. Si el promedio es mayor o igual a 9 pero menor que
    9.5 y el alumno es de preparatoria, entonces este podrá cursar 50
    unidades y se le hará un 10% de descuento. Si el promedio es mayor
    que 7 y menor que 9 y el alumno es de preparatoria, este podrá
    cursar 50 unidades y no tendrá ningún descuento. Si el promedio es
    de 7 o menor, el numero de materias reprobadas es de 0 a 3 y el
    alumno es de preparatoria, entonces podrá cursar 45 unidades y no
    tendrá descuento. Si el promedio es de 7 o menor, el numero de
    materias reprobadas es de 4 o mas y el alumno es de preparatoria,
    entonces podrá cursar 40 unidades y no tendrá ningún descuento. Si
    el promedio es mayor o igual a 9.5 y el alumno es de profesional,
    entonces podrá cursar 55 unidades y se le hará un 20% de descuento.
    Si el promedio es menor de 9.5 y el alumno es de profesional,
    entonces podrá cursar 55 unidades y no tendrá descuento. Obtener el
    total que tendrá que pagar un alumno si la colegiatura para alumnos
    de profesional es de \$300 por cada cinco unidades y para alumnos de
    preparatoria es de \$180 por cada cinco unidades.

9.  Que lea tres números diferentes y determine el número medio del
    conjunto de los tres números (el número medio es aquel número que no
    es ni mayor, ni menor).

Estructura de seleccion múltiple
--------------------------------

La estructura de selección múltiple <span>segun</span> permite elegir un
curso de acción de entre varios cursos de acción posibles, en base al
valor de una variable que actúa como <span>*selector*</span>. La
estructura compara el valor del selector con las constantes
<span>C1</span>, <span>C2</span>, …, <span>CN</span>. En el momento en
que se encuentra una coincidencia, se ejecuta la acción correspondiente
y se abandona la estructura.

La estructura se escribe del siguiente modo en pseudocódigo:

     segun <selector>
     inicio-segun
         caso <C1> : <acciones1>
                     fin-C1
         caso <C2> : <acciones2>
                     fin-C2
         caso <c3> : <acciones3>
                   .
                   .
                   .
         caso <CN> : <accionN>
                     fin-CN
         defecto   : <accionesDefecto>
                     fin-defecto
     fin-segun
