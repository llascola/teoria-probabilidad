
# Table of Contents

1.  [Introducción Toma Decisiones](#orgbbb9775)
    1.  [Introducción](#org4570750)
    2.  [Decisiones](#org5bc54de)
    3.  [Lenguaje de la estadistica en la toma de Decisiones](#org1b345c8)
        1.  [El ensayo de las Teorias](#org7772750)
        2.  [Que teoría sustentar?](#org297007b)
        3.  [Que errores podemos cometer ?](#org034c5fb)
2.  [La Estadística Descriptiva](#org03f3303)
    1.  [Tipos de variables](#org95bebb4)
    2.  [Analisis decriptivo para variables categóricas](#org5af4423)
    3.  [Análisis descriptivo para variables cualitativas](#org38e6315)
    4.  [Medidas descriptivas para variables categóricas](#orgde75fa9)
    5.  [Medidas descriptivas para variables cuantitativas](#org36465c3)
3.  [Probabilidad](#orgaa46e35)
4.  [Variables Aleatorias y Distribuciones](#org1d7ec59)
5.  [Variables Aleatorias Continuas](#org435f4ab)
6.  [Variables Aleatorias de Dim >= 2](#orgc0735f5)
7.  [Proceso de Poisson, Bernulli y Cadena de Markov](#orge9cad6d)



<a id="orgbbb9775"></a>

# Introducción Toma Decisiones


<a id="org4570750"></a>

## Introducción

La Estadistica y el Metodo Cientifico nos proveen un conjuto de  
principios y procedimientos para obtener y resumir la informacion  
para la **Toma de Decisiones**.

El metodo Cientifico comprende los siguientes pasos:

-   **Formular Teorias**
-   **Recolección de datos**
-   **Resumen y Analisis de Datos**
-   **Interpretacion de los resultados**

Estos pasos ocurren de manera cíclica. Se empieza siempre formulando
teorias, se recoleccionan datos, estos se analizan y se interpretan,
generando nuevo conocimiento y nuevas teorías sobre estos.


<a id="org5bc54de"></a>

## Decisiones

-   **<span class="underline">Simples:</span>:** Puedo cruzar la calle en esta interseccion?
-   **<span class="underline">Complejas:</span>:** Supon            gamos que quiero comprar un nuevo
    auto 0KM y decido hacerlo con la General Motors. La respuesta
    a las si                         guientes preguntas puede influir sobre la decision:
    Distintos modelos producidos en el corriente año, que modelo es
    más eficiente en cuanto a Km recorridos por litro de combustible,
    en precio ?


<a id="org1b345c8"></a>

## Lenguaje de la estadistica en la toma de Decisiones

Esta nueva terminología involucra frases, símbolos y definiciones especiales. El  
significado de una palabra es el lenguaje corriente puede ser diferente de cómo esa  
palabra está definida en el contexto de la Estadística. En esta Sección discutiremos la  
terminología estadística en el contexto del proceso de tomar decisiones. Hay muchas  
componentes en este proceso; incluye teorías, datos, una medida de “likeliness” y la  
posibilidad de errores.  


<a id="org7772750"></a>

### El ensayo de las Teorias

Competencia de teorías que sobre una población que deseamos investigar. Estas
teorías se denominan **Hipótesis Estadísticas**. Tenemos 2 tipos

-   ****H<sub>0</sub> -> Hipótesis nula**:** Afirmación de que nada está sucediendo, no existe diferencia, no hay cambios
    en la población. Es la creencia convencional, el status quo.
-   ****H<sub>1</sub> -> Hipótesis alternativa**:** Afirmación que el investifador espera que sea cierta. El cambio en la
    población que el investigador está buscando. Es la competencia a esa creencia.


<a id="org297007b"></a>

### Que teoría sustentar?

Si los datos son poco probables de ocurrir cuando la primer teoría es cierta
**rechazo** esta teoría y sustentamos la otra. Esto  no implica que la teoría
que sustentamos sea la cierta. La lógica detrás de la toma de decisión esta basada
en el concepto de **suceso raro**. Dado que la H<sub>0</sub> es en general, el status quo,
comenzamos **suponiendo que la H<sub>0</sub> es cierta**.

En general, la H<sub>1</sub> es el objetivo del investigador, puesto que la H<sub>0</sub> está tomada
como cierta. Cuando rechazamos H<sub>0</sub> en favor de H<sub>1</sub>, se dice que los datos conducen
a un test o ensayo **Estadisticamente significativo**, es decir, los datos son poco
probables de ser observados bajo el supuesto de que H<sub>0</sub> es cierta.


<a id="org034c5fb"></a>

### Que errores podemos cometer ?

-   ****Error tipo I**:** Error que se comete cuando se rechaza H<sub>0</sub> siendo cierta .(e<sub>I</sub>)
-   ****Error tipo II**:** Error que se comete cuando no se rechaza H<sub>0</sub> y es cierta la
    H<sub>1</sub>. (e<sub>II</sub>)

Tabla de consecuencias.

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-left" />

<col  class="org-left" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">&#xa0;</th>
<th scope="col" class="org-left">H<sub>0</sub> es verdadera</th>
<th scope="col" class="org-left">H<sub>1</sub> es verdadera</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">Sustentar H<sub>0</sub></td>
<td class="org-left">No hay error</td>
<td class="org-left">e<sub>II</sub></td>
</tr>


<tr>
<td class="org-left">Sustentar H<sub>1</sub></td>
<td class="org-left">e<sub>I</sub></td>
<td class="org-left">No hay error</td>
</tr>
</tbody>
</table>

-   **P(e<sub>I</sub>)::** Probabilidad de rechazar H<sub>0</sub> siendo ella cierta.
-   **P(e<sub>II</sub>)::** Probabilidad de no rechazar H<sub>0</sub>, cuando en realidad es cierta H<sub>1</sub>


<a id="org03f3303"></a>

# La Estadística Descriptiva

La **Estadistica** es la ciencia de recolectar, analizar y 
sacar conclusiones a partir de un conjunto de datos.
En este proceso se pueden diferenciar dos partes:

-   **<span class="underline">Estadistica descriptiva:</span>:** Organizar y resumir la información
    en tablas, gráficos y medidas resumen.
-   **<span class="underline">Estadística inferencial:</span>:** Sacar conclusiones o tomar decisiones.

Le llamaremos **población** al conjunto de objetos acerca del cual 
se desea obtener información. Y **muestra** es un subconjunto de la
población y será lo que se estudiará para sacar conclusiones. Estas
muestras deben ser respresentativas para obtener buenas conclusiones.

Una **variable** es una característica cuyo valor, o dato, puede cambiar de un 
objeto a otro. Los conjuntos de datos se diferencian según la cantidad
de variables observables, estos pueden ser univariado, bivariado o multivariado

Las medidas resumen que se obtienen de una población se denominan
**parámetro** y los que se obtienen a partir de una muestra se llama **estadistica**.


<a id="org95bebb4"></a>

## Tipos de variables

-   **<span class="underline">Categórica:</span>:** Cada observación pertenece a un conjunto de categorías. La característica fundamental
    a describir es el número relativo de observaciones en las distintas categorías.
-   **<span class="underline">Cuatitativa:</span>:** Cada observación toma valores numéricos que representan diferentes magnitudes.
    Con este tipo de variables se calculan las medidas resumen con excepción de las que no representan
    una cantidad o magnitud, ejemplo: código de área. Las característica a describir son el centro
    y la variabilidad o dispersión de los datos.
    Estas se dividen en
-   **<span class="underline">Discretas:</span>:** Cada valor que toma pertenece a un conjunto discreto, como los número enteros.
-   **<span class="underline">Continua:</span>:** Cada valor que toma pertenece a un conjunto continuo, como un intervalo.


<a id="org5af4423"></a>

## Analisis decriptivo para variables categóricas

-   **<span class="underline">Tablas de frecuencias:</span>:** Como cada observación cae en una categoría,
    podemos usar proporciones o porcentajes (frecuencias relativas) para resumir el número de observaciones.
    La proporcion es la cantidad de observaciones de esa categoria sobre el total de las observaciones. El
    porcentaje es la proporción multiplicado por 100.

<table border="2" cellspacing="0" cellpadding="6" rules="groups" frame="hsides">


<colgroup>
<col  class="org-left" />

<col  class="org-right" />

<col  class="org-right" />

<col  class="org-right" />
</colgroup>
<thead>
<tr>
<th scope="col" class="org-left">Categoría</th>
<th scope="col" class="org-right">Frecuencia</th>
<th scope="col" class="org-right">Frecuencia Relativa</th>
<th scope="col" class="org-right">Frecuencia Relativa Porcentual</th>
</tr>
</thead>

<tbody>
<tr>
<td class="org-left">Si</td>
<td class="org-right">51</td>
<td class="org-right">0.51</td>
<td class="org-right">51%</td>
</tr>


<tr>
<td class="org-left">No</td>
<td class="org-right">49</td>
<td class="org-right">0.49</td>
<td class="org-right">49%</td>
</tr>


<tr>
<td class="org-left">Total</td>
<td class="org-right">100</td>
<td class="org-right">1.00</td>
<td class="org-right">100%</td>
</tr>
</tbody>
</table>

-   **<span class="underline">Gráfico de torta:</span>:** Consiste en un círculo con sectores, donde cada sector es una categoria.
    El tamaño del sector es proporcional a su frecuencia relativa. Se utilizan cuando hay pocas
    categorías.

-   **<span class="underline">Gráfico de barras:</span>:** Consiste en barras, donde cada barra es una categoría. Las barras deben
    tener todas el mismo ancho y la altura depende de la frecuencia o frecuencia relativa de la Categoria.
    Se suelen utilizar para comparar las categorías.
-   **<span class="underline">Gráfico de Pareto:</span>:** Consiste en un gráfico de barras ordenadas por su frecuencia de forma 
    descendente. Este diagrama ayuda a mostrar el principio de Pareto, &ldquo;un pequeño numero de categorías 
    contiene a la mayoría de las observaciones&rdquo;.


<a id="org38e6315"></a>

## Análisis descriptivo para variables cualitativas

-   **<span class="underline">Gráfico de bastones:</span>:** Consta de bastones (barras sin ancho), los cuales se utilizan para representar
    datos numéricos discritos, los cuales se originan en base a un conteo. En el eje horizontal, se colocan
    los valores que toma la variable en estudio y en el eje vertical, la frecuencia de los valores.
-   **<span class="underline">Gráfico de puntos:</span>:** Cada observación se representa por un punto sobre la ubicación correspondiente a 
    su valor en una escala horizontal. Cuando un valor se presenta en mas de una ocación, se coloca por
    encima del anterior punto, esto nos da la frecuencia del valor. Se utiliza cuando el conjunto de datos 
    es pequeño ya que se muestran todas las observaciones.
-   **<span class="underline">Gráfico de tallo y hoja:</span>:** El gráfico se divide en dos partes, el tallo es la primera parte de número
    y es el primer dígito o digitos. La hoja es la última parte del npumero y son los digitos finales. Con estos 
    datos se puede obtener graficar de una manera sencilla la forma, dispersión y datos extremos o &ldquo;outliers&rdquo;,
    estos últimos son valores muy alejados del resto. Con los gráficos de puntos y de tallo y hoja es fácil 
    reconstruir los datos originales cuando se trata de un conjunto pequeño.
-   **<span class="underline">Histogramas:</span>:** Consta de barras para mostrar las frecuencias o frecuencias relativas de las variables.
    Una variable continua asume muchos valores distintos, lo que hace necesario dividir el rango de valores en
    intervalos mas pequeños. La cantidad de intervalos se calcula como (la raiz de n) = m y la amplitud 
    como (max-min)/m.

También se pueden utlizar intervalos de distinta amplitud cuando hay datos que tienen
frecuencias muy extremas (bajas o altas). Para este caso, se utiliza la densidad en el eje vertical 
se cacula como frecuencia relativa sobre ancho de ese valor.
La forma del histograma nos muestra la tendencia de la variable, esta puede ser:

-   **<span class="underline">Simetrico:</span>:** Si tanto, lado izquierdo como derecho mantienen una simetría respecto al centro.
-   **<span class="underline">Asimetricos:</span>:** Si la cola superior del histograma se prolonga más que la cola inferior.
-   **<span class="underline">Asimetría a la derecha o positiva</span>:** Si la cola derecha posee menor frecuencia que la izquierda.
-   **<span class="underline">Asimetría a la izquierda o negativa</span>:** Si la cola izquierda posee menor frecuencia que la derecha.


<a id="orgde75fa9"></a>

## Medidas descriptivas para variables categóricas

-   Frecuencias relativas
-   Moda


<a id="org36465c3"></a>

## Medidas descriptivas para variables cuantitativas

-   **<span class="underline">Medidas de posición central:</span>:** Se busca describir el centro o compararlo con el resto de los datos
    en relación al promedio y la mediana. El promedio tiene el problema de poder estar muy influido
    por las observaciones extremas, a diferencia de la mediana. El promedio toma en cuenta los valores y
    la mediana solamente la cantidad de observaciones.
-   **<span class="underline">Medidas de variabilidad:</span>:** Son medidas que describen el grado en el cual las observaciones se
    alejan del promedio.
    -   Rango = max - min.
    -   Desviaciones respecto de la media: Muestra que tan alejado está un dato de la media. Se obtiene 
        restándole a la media cada observación.
    -   Variancia muestral: Es la suma de las desviaciones de la media al cuadrado dividido por (n-1).
    -   Desvío estándar muestral: Es la raiz cuadrada positiva de la variancia muestral.
    -   Rango intercuartil: Es una medida de variabilidad resistente a los efectos de los outliers. Existen
        tres cuartiles, Q1 separa el 25% inferior del conjunto total, Q2 es la mediana que separa el 50% 
        del total y Q3 separa el 25% superior del resto. El rango intercuartil es Q3 - Q1. El gráfico que 
        muestra estos datos es el boxplot.


<a id="orgaa46e35"></a>

# TODO Probabilidad


<a id="org1d7ec59"></a>

# TODO Variables Aleatorias y Distribuciones


<a id="org435f4ab"></a>

# TODO Variables Aleatorias Continuas


<a id="orgc0735f5"></a>

# TODO Variables Aleatorias de Dim >= 2


<a id="orge9cad6d"></a>

# TODO Proceso de Poisson, Bernulli y Cadena de Markov

