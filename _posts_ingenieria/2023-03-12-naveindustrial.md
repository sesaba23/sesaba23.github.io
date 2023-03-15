---
title: Diseño de una nave industrial
author: sesaba23
date: 2023-03-12
category: sesaba
layout: post
published: true
---


## Diseño de una nave industrial: estructura

*Publicado: {{ page.date | date_to_string}} \| Autor: {{ page.author }}*

<div markdown=1 style="text-align: justify">

Sin ser ni mucho menos un experto, en el siguiente artículo voy a tratar de
describir el proceso seguido para el cálculo de una estructura de una nave industrial.  
Para facilitar el análisis, se ha elegido una estructura artículada a base de 
vigas metálicas para que sea lo más sencillo posible, aun sabiendo que este 
tipo de estructuras, está en desuso. En la actualidad se diseñan estructuras
prefabricadas de hormigón, más sencillas y rápidas de montar pero cuyo cálculo 
se basa en estructuras hiperestáticas más complejas de calcular.
En cualquier caso, son necesarios unos conocimientos mínimos de resistencia de
materiales y de mecánica de estructuras para poder entender las alternativas
constructivas planteadas.

Por simplicidad, no se han tenido en cuenta otros condicionantes, como puede ser
la estabilidad de la estructura ante el fuego, conforme el CTE DB-SI.

Sin más, empezamos:


<div markdown=1 style="border-width: 1px; border-style:dotted; border-color:grey; padding: 12px; background-color:lightgray">
**Tabla de contenidos:**

1. [Descripción de la actividad prevista](#1)  
2. [Programa de necesidades](#2)  
3. [Estructura](#3)  
    3.1. [Cimentación](#31)  
    3.2. [Estructura, justificación de la solución propuesta](#32)  
    3.3. [Justificación de las soluciones propuestas y análisis de alternativas](#33)  
        3.3.1. [ALTERNATIVA 1: Cubierta a base de pilares HEB y pórticos IP](#331)  
        3.3.2. [ALTERNATIVA 2: Cubierta a base de pilares HEB y cerchas articuladas tipo americana](#332)
4. [Envolvente](#4)  
</div>

<a id="1"></a>

### 1. Descripción de actividad prevista

Se trata de una IMPRENTA Y TALLER DE ARTES GRÁFICAS, principalmente servicios de impresión. 
Se contempla el almacenaje de materias primas para posteriormente y, previa manipulación, 
proceder a la impresión de documentos en formato papel: folletos publicitarios, 
pasquines, libros, etc.

El proceso de trabajo contempla las siguientes etapas:
1. Recepción de la materia prima, pedidos.
2. Almacenaje en pallets hasta su utilización.
3. Diseño y desarrollo del trabajo
4. Taller para impresión y pruebas; corte, si es necesario.
5. Preparación y expedición de los pedidos en almacenamiento de día.

Adicionalmente, se proyecta una pequeña zona de venta con sala de exposición. 
Para facilitar el proceso y mejorar los flujos de trabajo, se prevé 
una zona de almacenamiento del producto terminado para venta minorista y otra 
para mayorista, por lo que la nave se diseña para que sea completamente diáfana.

<a id="2"></a>

### 2. Programa de necesidades

La nave contará con módulo de oficinas en dos plantas; el resto de la planta baja
se destina a fabricación y almacén, así como una zona de exposición-comercial
y módulo de aseos y vestuarios. 

Cuadro resumen de superficies:

|Dependencia|Superf. construida (m²)|
|:----|:----:|
|Recepción Oficinas|25|
|Espacio de exposición|25|
|Despacho financiero y caja|10|
|Almacén de venta minorista|75|
|Aseos públicos|15|
|Comedor personal|25|
|Administración|50|
|Vestuarios|25|
|Despacho de dirección|25|
|**Superficie total oficinas:**|**275**|
|Muelle de Descarga|200|
|Almacén venta mayorista|200|
|Sala de pruebas de material|50|
|Sala de empaquetado|15|
|Despacho de control|25|
|**Superficie total Industrial:**|**625**|
|**SUPERFICIE TOTAL CONSTRUIDA**|**900 m²**|

<a id="3"></a>

### 3. Estructura

Se ha proyectado una estructura metálica articulada de acero S-275, con una 
estructura principal constituida a base de pilares HEB y vigas IPE sobre la que s
e apoyará una cubierta tipo cercha en celosía americana a dos aguas. Ésta, será 
simétrica de 5x2 tramos con perfiles en forma de “T” a base de perfilería “L” 
soldada y barras huecas con perfil cuadrado. Sobre la misma apoyarán correas de 
cubierta de acero conformado perfil omega con una separación máxima de 1,5 metros 
y luz de 5 metros.
La cubierta estará compuesta a base de panel sándwich con doble chapa de acero y 
relleno interior de espuma de poliuretano, fijada mediante tornillos a las correas
omega. Se considerará como cubierta ligera con un peso inferior a 100 kg/m2.

La estructura se cimentará sobre zapatas rectangulares excéntricas de hormigón 
armado en zona de medianería con el establecimiento colindante unidas mediante 
vigas centradoras y céntricas en el resto del perímetro, utilizando vigas de 
atado para dar mayor estabilidad.

La división de la zona administrativa se ha previsto mediante estructura secundaria
metálica a base de pilares HBE y vigas IPE, forjado mediante placas alveolares de 
hormigón pretensadas. Las divisiones verticales se realizarán mediante fábrica de 
ladrillo enfoscado en ambas caras.

Para el dimensionamiento y cálculo de la estructura y su cimentación se ha utilizado 
el [**software CYPE3D 2017**][1].

<a id="31"></a>

#### 3.1 Cimentación

La cimentación se basa en los siguientes elementos constructivos:
- <ins>Zapatas rectangulares excéntricas</ins> de hormigón armado, o zapatas de medianería: 
zapata donde el pilar que está apoyado sobre ella toca el límite del predio y,
por tanto, la carga no queda centrada en el cimiento. Se utilizan en paramentos
verticales adosados a otras naves.
- <ins>Zapatas centradas</ins>: utlilizadas donde no existe ningún problema espacial. 
También se pueden dimensionar como zapatas cuadradas centradas.
- <ins>Vigas de atado</ins>: elementos estructurales de hormigón armado que unen dos o 
más zapatas. Tienen como finalidad absorber las posibles acciones horizontales 
que pueden recibir los cimientos de la estructura, evitando, de esta forma, el 
desplazamiento horizontal relativo de uno respecto a otro.
- <ins>Vigas centradoras</ins>: se trata de un tipo de vigas de atado que además de 
arriostrar las zapatas, sirven de apoyo horizontal para zapatas muy excéntricas. 
Se encargan de mantener la zapata en equilibrio cuando sea necesario que se 
contrarreste el momento transmitido por el pilar. 

A partir de la estructura metálica se calculan las dimensiones de cada uno 
de los elementos de cimentación, teniendo en cuenta que en uno de los laterales 
deberá tener zapatas excéntricas desplazadas, con el fin de no invadir la parcela contigua. 

Por otro lado, se han realizado las comprobaciones de seguridad oportunas: 
separación máxima entre estribos, comprobación de armadura necesaria 
por cálculo a flexión compuesta, o separación máxima de la armadura longitudinal 
entre otras.

El suelo en contacto con el terreno se realizará con solera de hormigón de espesor 
15 cm. armado con mallazo 30x30x6. El forjado de la planta primera de la zona de 
oficinas a base de chapa colaborante con capa de hormigón de 10 cm.

<a id="32"></a>

#### 3.2 Estructura, justificación de la solución propuesta

Se ha optado por estructura metálica con pilares HBE-160B y vigas IPE-270,
sobre los que apoyan cerchas metálicas en forma de celosía americana simétrica 
a dos aguas de 5 tramos a base de perfilería soldada en forma de “T” y 
articulaciones interiores con perfilería cuadrada hueca tipo “SHS” 70x3.0.

Esta configuración permite que la nave quede completamente diáfana, lo que aporta 
versatilidad total para alojar el módulo de oficinas de dos alturas con 
estructura a base de pilares HBE-100 y vigas IPE-270.

Para el cálculo se ha tenido en cuenta el Código Técnico de la Edificación, 
Documento Básico Seguridad Estructural; para la consideración de las distintas 
cargas el DB SE-Acciones en la edificación. 

Las principales cargas se pasan a describir a continuación:

1.	<ins>Cubierta</ins>: 
- Panel tipo sándwich con aislamiento térmico y peso 0,1 KN/m2.
- Sobrecarga de uso 0,4 KN/m2 según tabla 3.1 CTE DB-SEA, categoría de uso G1, cubiertas 
ligeras sobre correas (sin forjado) accesibles únicamente para conservación.
- Nieve: 0,2 KN/m2
2.	<ins>Oficinas</ins>: 
- Peso propio 3 KN/m2. Forjado unidireccional, luces hasta 5 metros; 
Grueso total < 0,28 m, Según la tabla C.5 del Anejo C
- Sobrecarga de uso total 3 KN/m2: 2 KN/m2 debido a la carga administrativa, 
según tabla 3.1. categoría de uso B, zonas administrativas y 1 KN/m2
tabiquería asimilable a viviendas, según apartado 2.1.

3.	<ins>Fachadas laterales más frontal</ins>: (1+1) + (1+1) no concomitantes: 
- Viento 0,6 KN/m2.

<ins>Cargas por nieve</ins>: según el apartado 3.5.1 del CTE DB-SEA. Se utiliza la siguiente fórmula:

$$ q_n = \mu·S_k = 1 * 0.2 = 0.2 { KN \over m²} $$

Siendo:
- µ el coeficiente de forma de la cubierta: según el apartado 3.5.3 toma el 
valor de 1 debido a que la cubierta tiene inclinación menor o igual que 30º; 
en nuestro caso 21,8º.
- S<sub>k</sub>: valor característico de la carga de nieve sobre el terreno 
horizontal según el apartado 3.5.2, tabla 3.8 que para, por ejemplo, Almería
corresponde un valor de 0,2 KN/m2.

<ins>Cargas debidas al viento</ins>: se utiliza el apartado 3.3.2 del CTE DB-SEA, a saber:

$$ q_e = q_b · q_e · q_p = 0.5 * 1.7 *  0.7 = 0.595 \approx 0.2 { KN \over m²} $$

Siendo:
- q<sub>b</sub>  la presión dinámica del viento: de forma simplificada, este valor para 
toda España puede tomarse como de 0,5 KN/m2.
- q<sub>e</sub> es el coeficiente de exposición, variable con la altura de la localidad. 
Según la tabla 3.4 para edificios hasta 9 metros de altura en zonas industriales 
su valor puede tomarse como de 1,7.
- q<sub>p</sub>  es el coeficiente eólico o de presión, que depende de la forma y orientación 
de la superficie respecto del viento. Si bien su elección no es trivial, 
por simplicidad se ha escogido un valor de 0,7 para una anchura de nave de 
20 metros y una altura a mitad de cumbrera de 8,5 metros.


<a id="33"></a> 

#### 3.3 Justificación de las soluciones propuestas y análisis de alternativas


<a id="331"></a>

##### 3.3.1 ALTERNATIVA 1: Cubierta a base de pilares HEB y pórticos IP

Se contempla una solución tipo de estructura a base de los siguientes elementos:

- Pilares HEB-160 exteriores y pilares centrales HEB-200.
- Vigas de pórticos IPE 220 y vigas de unión entre pórticos IPE 270.
- Correas IPE 270.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/1-seleccion-material.jpg)
{:refdef}

En este proyecto se utiliza acero Laminado S-275. 
Una vez diseñada la estructura se obtiene una medición del peso total del 
material utilizado de aproximadamente 40.000 Kg.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/2-estructura.jpg)
{:refdef}

A continuación, se muestra la estructura diseñada:

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/3-estructura-3d.jpg)
{:refdef}

Si bien tiene la ventaja de que los esfuerzos axiles sobre los pórticos de 
cubierta son mínimos, la principal desventaja, es que para que las secciones de 
los pilares IPE de los pórticos no sean excesivas, es necesario colocar pilares 
en el centro. Esto limita mucho la distribución interior puesto que NO permite 
un espacio totalmente diáfano, algo que puede ser un problema cuando pretendemos 
destinar gran parte de la superficie a zona de almacenamiento.  

Otro inconveniente característico de estos pórticos es el gran momento flector 
que presentan alrededor su “eje x”, debido a la longitud máxima de cada viga 
(10 metros). Esto conlleva deformaciones importantes en la zona intermedia de 
cada uno de los paños de cubierta, pudiendo llegar a los 22,35 milímetros. 
Si por necesidades funcionales eliminásemos algún pilar central, la deformada 
se dispararía. Para evitarlo, necesitaríamos aumentar considerablemente la 
sección de las vigas, lo que incrementa considerablemente la cantidad de acero 
a emplear y, por tanto, el coste de la estructura.

En la siguiente figura se representa un perfil IPE típico donde se aprecian las 
secciones y sus distintos momentos de inercia, así como los módulos resistentes por eje:

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/4-IPE.jpg)
{:refdef}

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/5-IPE-caracteristicas.jpg)
{:refdef}

Imagen representativa de la deformada incluyendo pilares centrales en todos 
los pórticos. Observar que la deformada máxima es de 22,35 mm, valor nada despreciable.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/6-deformada-estructura.jpg)
{:refdef}

Gráfica de esfuerzos axiles. Los esfuerzos en cubierta son despreciables.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/7-axiles-estructura.jpg)
{:refdef}

Gráfica de momento flectores en el eje “x”. Los pórticos presentan un momento elevado debido a la distancia entre pilares lo que obliga a aumentar la sección del perfil.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/8-momentos-estructura.jpg)
{:refdef}

Hipótesis de deformada eliminando dos pilares centrales de la zona de descarga y almacenamiento mayorista por necesidades operativas. Se mantienen las secciones de perfiles. La deformada en los pórticos de cubierta puede alcanzar los 44,95 mm, valor que no es asumible, por lo que necesitaríamos aumentar la sección de los pilares IPE considerablemente.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/9-hipotesis-1-deformada.jpg)
{:refdef}

<a id="332"></a>

##### 3.3.2 ALTERNATIVA 2: Cubierta a base de pilares HEB y cerchas articuladas tipo americana

Primero analizamos la estructura articulada utilizada. Como ya se ha dicho, se trata
de una estructura simétrica a dos aguas tipo cercha, modelo americano, con 5 tramos. 
La ventaja de este tipo de estructuras es que permite luces mucho más amplias dado 
que no presentan momento flector; todas las barras trabajan con esfuerzos axiles.

Se ha realizado un cálculo aproximado de los nudos; Sin bien el cálculo conviene 
realizarlo *a mano* con cargas en cada uno de los nudos, se ha creído más conveniente 
simularlo con una aplicación especifica. Las cargas se sitúan donde idealmente 
se apoyarán las correas de cubierta. Para facilitar el cálculo, se han utilizado cargas 
puntuales de 1 kN/m.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/10-portico.jpg)
{:refdef}

Si bien por falta de espacio en la figura no se aprecian los valores, 
se observa que las barras superiores están trabajando a compresión con axil máximo
en la zona central de 10 KN (color rojo claro), aumentando según nos acercamos a 
los extremos hasta los 17 KN.  
La perfilería inferior trabaja a tracción con valores máximos de 16 KN en los extremos
(color azul oscuro). Las barras interiores apenas trabajan (entre 0 en los extremos, 
y 5 KN en el central), distribuyéndose los esfuerzos de tracción y compresión 
alternativamente, evitando que las barras perimetrales presenten momentos.
Para diseñar este tipo de estructura se ha utilizado perfiles en “T” mediante 
dos perfiles “L” con unión soldada para las barras perimetrales que forman el 
triángulo exterior (130x90x10 en la parte superior y 100x65x0,9 en la inferior). 
Se utilizan barras interiores con perfil hueco cuadrado modelo “SHS” 60x3.0. 
Esta perfilería tiene la ventaja de que presentan buenos momentos de inercia 
con un peso reducido, permitiendo su uso en esta estructura articulada que, 
como se ha dicho, idealmente no está sometida a momentos flectores.

Se muestran a continuación las tablas de dichos perfiles:

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/11-tabla2A16.jpg)
{:refdef}

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/12-tabla2A22.jpg)
{:refdef}

Para las correas de cubierta se han contemplado tres opciones:

1. <ins>Perfiles “IPE”</ins>: las dimensiones calculadas son las mismas que 
para la alternativa 1 (IPE 270). El peso de la estructura apenas se reduce.
2. <ins>Perfiles “Z”</ins>. Si bien esta opción es la más utilizada para esta 
tipología de naves, la separación de 5 metros que se ha propuesto entre pórticos 
hacía que, para las secciones existentes en el mercado, el programa indicase 
que *se ha superado la esbeltez máxima*. Si bien un estudio exhaustivo del caso 
podría indicarnos que este error no es crítico, se optó por otra alternativa.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/13-tabla2A36.jpg)
{:refdef}

3. <ins>Perfiles Omega “W”</ins> con acero conformado 130x90x10: este perfil presenta 
una buena relación entre momento de inercia y dimensiones, con un peso mínimo. 
Los flancos inferiores permiten reforzar su módulo resistente y además ahorra 
soldaduras a los perfiles “T” de los pórticos, permitiendo su unión mediante tornillería. 
Ésta es la opción elegida.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/14-tabla2A35.jpg)
{:refdef}

Para evitar que la estructura forme un mecanismo, se utilizan cruces de *“San Andrés”* 
mediante tirantes macizos de sección circular R15 en extremos de fachadas.

Para resolver los nudos interiores, se han utilizado nudos con coeficiente de 
empotramiento parcial del 50%, solución intermedia entre nudos empotrados y 
completamente articulados. Esta alternativa facilita enormemente el control de 
la dirección de obra.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/15-estructura-3d.jpg)
{:refdef}

La deformada conseguida con esta alternativa es mínima (4,18 mm en su punto máximo) 
un 79% inferior a la alternativa 1 sin utilizar pilares internos, es decir,
con un espacio interior totalmente diáfano.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/16-deformada-estructura.jpg)
{:refdef}

En las siguientes figuras se muestran los esfuerzos axiles de la estructura de cubierta, coincidente con lo previamente calculado. Denotar que los esfuerzos axiles de los pilares se deben a las cargas del viento en un único sentido (no concomitantes).

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/17-axiles-estructura.jpg)
{:refdef}

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/18-axiles-frontal.jpg)
{:refdef}

En las siguientes figuras se aprecia que los momentos flectores son prácticamente 
inexistentes en cubierta. Se denota que en la segunda y tercera imagenes, se ha 
escalado por un factor de “10” para poder observar momentos en las barras de cubierta.
Esos pequeños momentos flectores entre barras del triángulo superior son debidos 
a que el apoyo de las correas no está exactamente sobre los nudos de barras interiores 
debido a las limitaciones geométricas impuestas en el diseño (distancia de 30 cm 
a faldones de cubierta para el espacio de los canalones de la red de saneamiento 
y máxima distancia entre ellas de 1,5 metros). No obstante, su valor se puede 
considerar despreciable.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/18-axiles-frontal.jpg)
{:refdef}

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/19-momentos-estructura.jpg)
{:refdef}

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/20-momentos-estructura-2.jpg)
{:refdef}

Figura que muestra las reacciones en los nudos de apoyo con el terreno.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/22-apoyos-terreno.jpg)
{:refdef}

**El peso total del acero utilizado es el que se muestra a continuación, observándose**
**el ahorro de peso y, por tanto, ahorro económico comparado con la estructura clásica de la alternativa 1**:

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/23-tabla-acero.jpg)
{:refdef}

> Se reduce el peso 27 toneladas con respecto a la alternativa 1 (40 Tn), es decir, un 21%
>
{: .block-tip  }

Detalles en 3D de la estructura planteada donde se pueden apreciar los perfiles Omega de la estructura de cubierta y el espacio diáfano en el interior de la nave:

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/nave-estructura/24-estructura-3d-frontal.jpg)
{:refdef}

Se aprecia que los apoyos de las correas no están exactamente sobre los nudos de la cercha. 
No obstante, los momentos flectores son despreciables.
La estructura de la planta de oficinas se resuelve con pilares HEB 100 y vigas IPE 270.
No se considera necesario entrar en mayor detalle debido a su simplicidad. 
En la figura superior se puede observar la estructura al fondo.

<a id="4"></a>

### 4. Envolvente

Los materiales utilizados en los cerramientos responderán a las necesidades de 
la propia edificación. Deberán tener distintas características para cumplir 
con las funciones que de ellos se esperan como pueden ser aislamiento acústico o térmico.

#### 4.1 Fachadas

Para el diseño de fachadas se considera cerramiento ligero con basamento de 
hormigón prefabricado de espesor 25 cm, con una altura de 1,5 metros sobre la rasante. 
El resto de la altura hasta faldón de cubierta, se proyecta a base de panel sándwich 
de 50 mm de espesor sobre estructura de cerchas de fachada en cara exterior.

Las cerchas de fachada serán de perfil C250S, el remate con el faldón o peto de 
cubierta se realizará con chapa simple interior con espacio suficiente para la 
instalación de canalón oculto.

En la zona de oficinas se instalará trasdosado interior de pladur con aislamiento 
de poliestireno de 30 mm de espesor.

Para huecos de fachada se prevé carpintería de PVC a una altura de 1 metro sobre
 forjado de planta primera y 100x120 cm de dimensiones con cristal tipo Climalit 4/10/4 mm.

La justificación pasa por la elección de los distintos componentes de acuerdo
con las especificaciones del promotor y con las condiciones ambientales de la zona, 
consiguiendo que la transmitancia total de la fachada no supere los límites que, 
por zona, le corresponden a nuestra nave industrial.

Se han escogido paneles sándwich con un coeficiente de transmitancia de 0,27 W/m2K
y tornillería escondida.

Cumplirá lo indicado en el CTE, Documento Básico Ahorro de Energía y el Reglamento
de Instalaciones Térmicas en el módulo de oficinas.

#### 4.2 Cubiertas

Se proyecta a base de panel sándwich de 80 mm de espesor sobre correas de cubiertas 
tal y como se ha especificado en el cálculo estructural.

<br>

---

Hasta aquí este artículo. En proximas entregas incluiré el resto de instalaciones
típicas de una nave industrial: evacuación de aguas, seguridad en caso de incendio,
etc.


</div>

*[CTE DB-SEA]: Código Técnico de la Edificación, Documento Básico Seguridad Estructural
*[CTE DB-SI]: Código Técnico de la Edificación, Documento Básico Seguridad contra Incendios

[1]: https://info.cype.com/es/software/cype-3d/