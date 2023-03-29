---
title: Cocinas Industriales
author: sesaba23
date: 2023-03-24
category: cte-db-si
layout: post
published: true
---
## Diseño de campanas extractoras y conductos de ventilación
*Publicado: {{ page.date | date_to_string}} \| Autor: {{ page.author }}*

---
<div markdown=1 style="text-align: justify">

<div markdown=1 style="border-width: 1px; border-style:dotted; border-color:grey; padding: 12px; background-color:lightgray">
**Tabla de contenidos:**

1. [Cálculo del caudal de extracción selección de campanas y conductos](#1)
2. [UNE 60670-6:2014](#2)
3. [CTE-DB-SI](#3)
4. [Conclusiones](#4)
</div>

<br>

<a id="1"></a>

### Cálculo del caudal de extracción, selección de campanas y conductos

Para calcular el caudal de extracción de la campana con objeto de evacuar
vahos (vapores de grasas, aceites y agua) que emanan durante el cocinado de alimentos, así como los eventuales productos de la combustión, además de eliminar calor, nos podemos remitir a la norma **UNE-100165:2004 *Climatización. Extracción de humos y ventilación de cocinas***.

Cómo la propia norma indica, es importante que el proyectista estudie el
equilibrio entre los caudales de aire extraidos de la cocina, a través de la
campana, y los locales adyacentes como comedores, con el fin de que la
cocina quede en ligera depresión con respecto a éstos no superior a 5 Pa
para evitar el paso de olores y la posibilidad de entrada de insectos y polvo.

Un condicionante obvio pero conviene resaltar, es que el conducto de extracción de la campana debe ser independiente de cualquier otro uso y no puede ser atravesado por elmentos ajenos a la evacuación de dicho aire.  
Además, como regla general, en la mayoría de municipios se suele obligar a que el conducto desemboque en cubierta, prohibiéndose su salida a fachadas o patios interiores. Además, suele obligarse a que su desembocadura quede situada a una altura mínima sobre edificaciones próximas situadas en un radio de acción que tipicamente suele ser de al menos 10 o 15 metros.

El apartado 5 de la citada norma propone un método sencillo para cálcular
el caudal óptimo en función del aŕea, la potencia térmica y la dimensión lineal de los aparatos de cocción a los que da servicio. 

No obstante, voy a hacer uso de la aplicación [**QuickFan Selector**][2] desarrollada por SODECA y que ofrece gratuitamente desde su web.  
Esta aplicación, nos facilita diversas herramientas para multitud de situaciónes, permitiéndonos calcular el caudal de extracción necesario de la campana conforme a las citada norma UNE. Además, permite calcular las pérdidas de carga del conducto de extracción y la selección del extractor más adecuado. Todo ello de una manera ágil y rápida, con unos conocimientos mínimos, reduciendo la posibilidad de errores.

> Conviene tener en cuenta que también se regula el caudal de aire extraído
> en la Norma UNE 60670-6:2014 aplicando la siguiente fórmula:
>
> $$ q \ge 10 \times \text{A} + 2 \times \sum Q_n $$  
>
> donde:
> * q es el caudal de aire, en m³/h
>* A es la superficie en planta del recinto en m²
> * $\sum$ Q<sub>n</sub> es el sumatorio de los poderes caloríficos de 
> cada aparato de cocción.
>
> En los cálculos justificativos finales habría que considerar el mayor caudal
> obtenido conforme a ambas Normas. No obstante, como
> *a priori* no concocemos la superficie del recinto de cocina, en este 
> artículo consideraremos unicamente el caudal obtenido aplicando la Norma
> UNE-100165:2004.
{: .block-warning }

La norma UNE propone también una serie de recomendaciones para **situar la campana**. Muchas de ellas las recoge el CTE DB-SI siendo de obligado
cumplimiento como más adelante se verá. A destacar las siguientes:
- El borde inferior debe ser instalado a una altura máxima de 2 metros del suelo,
- Debe dimensionarse de manera que sobresalga 15 cm como mínimo sobre la 
proyección en planta de los aparatos de cocción, por sus lados accesibles no adosados a paredes.
- Debe estar dotada de filtros metálicos para la retención de grasasy aceites
con una eficacia $\ge$ 90% en peso.
- La velocidad media de paso a través de los elementos filtrantes debe estar
comprendida entre 0,8 m/s y 1,2 m/s, con pérdidas de presión entre 10 y 40 Pa, a filtro limpio y sucio respectivamente.
- Los filtros se instalarán con una inclinación de entre 45º y 60º sobre la horizontal para facilitar su decantación sobre la bandeja de recogida.
- Los filtros deben estar separados más de 1,2 metros de fuegos abiertos y más de 0,5 m de focos de calor de otro tipo.
- La bandeja de recogida de grasas debe estar conectada a un recipiente cerrado de capacidad menor de 3 litros, por razones de seguridad.

La Norma también hace **recomendaciones sobre materiales**:
- Las campanas deben estar construidas con materiales M0 no porosos,
Lo conductos deben dimensionarse con una velocidad mínima de 8 m/s para
reducir el riesgo de deposición de sustancias grasas en la red.
- Igualmente las curvas deben tener un radio de curvatura no menor de 1,5 veces el diámetro hidráulico del conducto.
- Los conductos serán preferiblemente de sección circular de chapa de acero
negro o inoxidable de 1,5 mm de espesor, con juntas soldadas de continuidad y provistos de juntas de dilatación para un salto de temperatura de 1000 K.
- Deben disponerse registros de inspección de cierre hermético cada 3 metros, así como en cambios de dirección mayores de 30º, derivaciones y conexión al ventilador.
- El ventilador debe situarse al final de la red de conductos.
- Los ventiladores deben ser de la clase F-400. 

Por último indicar que la Norma UNE indica que es recomendable instalar un separador de grasas y aceites arrastrados por los humos.

#### Cálculo del caudal en función de las dimensiones de la campana

El primer paso en el diseño de la evacuación de humos de la cocina es seleccionar la campana. Su tamaño determinará los caudales recomendables
de extracción. Como ya hemos dicho, utilizaré la aplicación *QuickFan Select*, teniendo en cuenta los siguientes condicionantes:
- Instalacción de **campana industrial básica** de acero inoxidable,
- Aunque existen multitud de dimensiones, el fondo se va a considerar constante, **90 cm** suficiente para cubrir una cocina de tamaño medio,
- Cocina a gas, por ser más restrictiva que las cocinas eléctricas y de uso más extendido.
- 1,20 metros de distancia a los fuegos,
- Se situara sobre una pared, disponiendo de tres caras abiertas.

En la siguiente tabla se resumen los cálculos para obtener los caudales
de extracción en función del tamaño de la campana, así como el diámetro
recomendable del conducto o chimenea:

|Largo <br>(cm)|Q<sub>térmico</sub> <br>(m³/h)|$\phi_t$ <br>(mm)|Q<sub>mínimo</sub> <br>(m³/h)|$\phi_{min}$ <br>(mm)|
|:---:|:---:|:---:|:---:|:---:|
|100|2430|293,2|**3024**|327|
|120|2916|321,1|**3240**|338,5|
|150|**3645**|359|3564|355|
|170|**4131**|382,2|3780|365,6|
|200|**4860**|414,6|4104|381|
|220|**5346**|434,8|4320|390,9|
|250|**6075**|463,5|4644|405,3|

Se señala en negrita el valos del mayor caudal para cada longitud de campana que es el que se utilizará para calcular las pérdidas de carga. No obstante, para seleccionar el punto de operación de la caja de ventilación, admitiré caudales comprendidos entre 
ambos valores.

#### Selección del conducto

El siguiente paso consiste en seleccionar la sección del conducto que dará
servicio a la campana de extracción conduciendo los vapores procedentes
de la preparación de alimentos al exterior. Para ello,
vamos a considerar las siguientes restricciones:
- Se contemplan dos casos: un edificio de 5 plantas (18 m) y otro de 11 (36 m),
- Velocidad máxima del aire en el conducto: 12 m/s,
- Velocidad mínima 7 m/s,
- Interior del conducto terminado en chapa de acero galvanizado,
- Para calcular la pérdida de carga se han cosiderado un máximo de 3 codos de 90º y la posible reducción en la conexión a la caja de ventilación,
- Se selecciona el diámetro más pequeño posible teniendo en cuenta que la mayoría de edificios cuentan con locales con previsión de huecos de fábrica o incluso chimeneas a cubierta, pero con dimensiones reducidas.
- Los cálculos se refieren a cajas de ventilación instaladas en cubierta
como la propia Norma UNE recomienda, es decir, funcionando en aspiración.
En el caso de instalarlas junto a la campana de ventilación, funcionando
en impulsión, el punto de operación de la caja del motor cambia, obteniendo valores menos favorables.
- Los modelos de caja de ventilación con denominación ["CVT"][3] se refieren a cajas para instalación en cubierta sobre el conducto vertical. La conexión a conducto es de diámetro 500 mm.
- Lo modelos de caja de ventilación con denominación ["CJTHT"][4] se refieren a cajas de ventilación con posibilidad de instalar en cubierta o sobre campana. El diámetro de la conexión a conducto es de 565 mm.

{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/cocinas/cajas-ventilacion.png)
{:refdef}
<div markdown=1 style="text-align: center">
Extractor centrífugo de tejado mod. CVT (izq) y ventilador helicoidal con caja mod. CJTHT (der)
</div>

<br>
**CASO 1: Edificio de 5 plantas (h = 18 m)**:

|Q (m³/h)|D (mm)|P<sub>c</sub> (mmca)|v (m/s)|Caja Vent|Pt (mmca)|L<sub>w</sub> (dBA)|L<sub>p</sub> (dBA)|Qs (m³/h)|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|3024|300|17,53|11,88|CVT-450-6T|27,27|67|40|3745|
|3240|350|10,77|9,35|CJTHT-45-4T-26º|13,28|70|49|3309|
|3645|350|13,56|10,52|CVT-450-6T|22,27|68|41|4541|
|4131|350|17,33|11,93|CVT-450-6T|22,22|68|41|4547|
|4860|400|14,22|10,74|CVT-450-6T|15,03|70|49|4366|
|5346|400|17,15|11,82|CVT-450-6T|17,48|69|42|5150|
|6075|550|6,921|7,1|CJTHT-45-4T-38º|14,37|72|51|6363|

<br>

**CASO 2: Edificio de 11 plantas (h = 36 m)**:

|Q (m³/h)|D (mm)|P<sub>c</sub> (mmca)|v (m/s)|Caja Vent|Pt (mmca)|L<sub>w</sub> (dBA)|L<sub>p</sub> (dBA)|Qs (m³/h)|
|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|:---:|
|3024|300|27,12|11,88|CVT-450-6T|30,93|67|40|3198|
|3240|350|15,79|9,35|CVT-450-6T|25,7|68|41|4055|
|3645|500|4,6|5,157|CJTHT-45-4T-14º|7,23|71|50|3879|
|4131|500|5,869|5,84|CJTHT-45-4T-18º|9,67|70|49|4270|
|4860|500|8,05|6,875|CJTHT-45-4T-26º|13,23|70|49|5008|
|5346|550|6,75|6,25|CJTHT-45-4T-26º|11,96|70|49|5325|
|6075|600|6231|5,968|CJTHT-45-4T-26º|13,72|72|51|6369|

Donde:
* Q [m³/h]: caudal teórico máximo calculado según UNE-100165:2004
* D [mm]: Diámetro mínimo recomendado para el Caudal indicado
* P<sub>c</sub>: Perdida de carga en el conducto
* v [m/s]: velocidad media del vapor en el interior del conducto
* Caja Vent.: Caja de Ventilación elegida; catálogo SODECA
* P<sub>t</sub> [mmca]: Perdida de Carga total en el punto de operación del ventilador; P<sub>t</sub> = P<sub>e</sub> + P<sub>d</sub>.
* L<sub>w</sub> [dBA]: Nivel de potencia sonora 
* L<sub>p</sub> [dBA]: Nivel de presión sonora calculada a 3 metros en campo libre.
* Q<sub>s</sub> [m³/h]: Caudal que proporciona la caja de ventilación en el punto de operación. 

* P<sub>e</sub>: Presión estática, valor de la fuerza que ejerce el aire sobre las paredes del conducto en sentido perpendicular a ellas.
* P<sub>d</sub>: Presión dinámica, fuerza por unidad de superficie provocada por el movimiento del aire en el sentido del movimiento.

###### Conclusiones:

La campana insdustrial más pequeña (100 x 90 cm), aplicando la norma UNE 100165:2004, requiere un caudal mínimo de 3024 m³/h, caudal relativamente pequeño. Para este caudal, si lo que pretendemos es que la velocidad máxima sea de 12 m/s, el conducto debe tener al menos un diámetro de 300 mm. Según mi experiencia, los locales comerciales ubicados en los bajos de edificios en altura que tienen previsión de conductos a cubierta, suelen contar con secciones de diámetros entre 300 y 350 mm, 400 mm con mucha suerte.  
Con estas condiciones, la elección de extractores es muy limitada, llegando a reducirse en muchos casos a la instalación de un extractor centrífugo en el tejado; es muy posible que esta solución no sea posible por limitaciones fícicas.  
La elección es tan limitada debido a las altas perdidas de carga que se generan en conductos con secciones tan pequeñas como consecuencia de las altas velocidades, forzando que las los motores funciones por encima del punto de operación recomendado reduciendo su vida util y aumentando su consumo; además, aumentará considerablemente la emisión sonora de ruido e incluso se pueden generar vibraciones, tanto en la propia caja de ventilación como en el conducto.  
Otro inconveniente a tener en cuenta es que a velocidades altas, se pueden dañar las paredes del conducto por rozamiento, provocando fugas y filtraciones; si el conducto discurre por el interior de una edificación, 
nos podemos hacer una idea del problema que puede suponer.  
A medida que aumentamos la altura de la evacuación, como es lógico, las
pérdidas de carga aumentarán.

A tenor de los resultados obtenidos, lo recomendable sería contar con secciones de diámetro de al menos 500 mm. Esto nos permitiría instalar cajas de ventilación con aĺabes configurables a distintos ángulos, permitiendo en puntos de operación con valores de presión más bajos, reduciendo el consumo y la potencia acústica emitida.

Teniendo en cuenta lo anterior, al menos en locales comerciales situados en bajos de edificios en altura, si estos disponen de conducto de evacuación, nos tenemos que asegurar de que su sección es suficiente para las futuras necesidades. Si el local no dispone de conducto de evacuación y pretendemos conducirlo a cubierta por fachada o por patio interior, además de necesitar la autorización de la comunidad de propietarios, habrá que tener en cuenta que su tamaño puede ser considerable. Además, si dicurre a menos de 1,50 metros de huecos de fachada éste deberá ser EI-30, como más adelante se verá.

> En resumen, que el local disponga de **un conducto de evacuación de humos a cubierta 
> adecuado y de sección suficiente es un factor determinante** si se pretende ejercer 
> cualquier actividad donde sea necesaria una campana extractora de humos para una 
> cocina, por ejemplo en establecimientos de hosteleria. De hecho, un mal diseño 
> suele se fuente de problemas con la vecindad, generando molestias por olores 
> debidos a filtraciones, por ruidos, e incluso por vibraciones. 
{: .block-tip }


<a id="2"></a>

### UNE 60670-6:2014. Instalaciones receptoras de gas suministradas a una presión máxima de operación (MOP) inferior o igual a 5 bar. Parte 6: Requisitos de configuración, ventilación y evacuación de los productos de la combustión en los locales destinados a contener los aparatos a gas.

Según esta Norma, en el caso de que se instalen aparatos de gas (aparatos tipo A, de circuito abierto y evacuación no conducida), la cocina debe tener un volumen bruto mínimo en función del poder calorífico total de los aparatos de cocción ($\sum$ Q<sub>n</sub>):
- Si $\sum$ Q<sub>n</sub> $\le$ 16 kW ➡ 8 m³
- Si $\sum$ Q<sub>n</sub> $\gt$ 16 kW ➡ $\sum$ Q<sub>n</sub> - 8 m³
- En edificios ya construidos, si no es posible cumplir lo anterior, se admiten 6 m³.

Además, si $\sum$ Q<sub>n</sub> $\gt$ 30 kW, se debe disponer de un **sistema de extracción mecánica** de aire que garantice la renovación continua durante el funcionamiento de los aparatos. Esta condición se cumplirá siempre, puesto que, como hemos comentado, todas las cocinas deben disponer de una campana de extracción. Sin embargo, también hay que
incluir un **sistema de corte de gas por fallo del sistema de extracción**, que interrupta el suministro en caso necesario que consistirá en una electroválvula de rearme manual, normalmente cerrada, accionada mediante un interruptor de flujo situado en el conducto de extracción.

En cualquier caso, si la relación entre el volumen del local en m3 y el consumo calorífico total en kW es mayor que 10, no es necesario un sistema de extracción del gas.

Lo anterior, se refiere a la extracción mecánica de los vapores generados durante el cocinado y es independiente de los requisitos de ventilación necesarios por contener aparatos de gas tipo A tanto en el Reglamento de Combustibles Gaseosos, como en la norma UNE.


<a id="3"></a>

### CTE DB-SI; Cocinas

#### Sección SI-1, Propagación Interior

Las <ins>COCINAS</ins> se consideran una zona de riesgo especial según:

**Tabla 2.1. Clasificación de los locales y zonas de riesgo especial integrados en edificios.**

|:----|:----|:----|:----|
|Cocinas en cualqier edificio o establecimiento:|Riesgo Bajo|Riesgo Medio|Riesgo alto|
|Según potencia instalada|20$\lt$P$\le$30 kW|30$\lt$P$\le$50 kW|P$\gt$50 kW|

<div markdown=1 style="text-align: right">
*Ver notas (1) y (2)*
</div>

<ins>NOTA 1:</ins>
Para determinar la Potencia se consideran los aparatos destinados DIRECTAMENTE a la peparación de alimentos y que puedan probocar ignición.  
Freidoras y Sartenes basculantes se computan a razón de 1 kW por litro de capacidad.  
En usos DISTINTOS de HOSPITALARIO Y RESIDENCIAL PÚBLICO NO se considerán locales de riesgo especial:  
**Las COCINAS cuyos aparatos estén PROTEGIDOS con un sistema automático de extinción siempre que la P≤50 kW**.   
No obstante, también tienen que cumplir con la NOTA 2

<ins>NOTA 2:</ins>
Sistemas de extracción de humos de cocinas deben cumplir:
- Las campanas deben estar separadas al menos 50 cm de cualquier material que no sea A1.
- Los conductos deben ser independientes de toda otra extracción o ventilación y exclusivos para cada cocina. Deben disponer  de  registros  para  inspección  y  limpieza  en  los  cambios  de  dirección  con  ángulos  mayores  que  30°  y  cada  3  m  como  máximo de tramo horizontal. Los conductos que discurran por el interior del edificio, así como los que discurran por fachadas a menos de 1,50 m de distancia de zonas de la misma que no sean al menos EI 30 o de balcones, terrazas o huecos practi-cables tendrán una clasificación EI 30.  
No deben existir compuertas cortafuego en el interior de este tipo de conductos, por lo que su paso a través de elementos de compartimentación de sectores de incendio se debe resolver de la forma que se indica en el apartado 3 de esta Sección.
- Los filtros deben estar separados de los focos de calor más de 1,20 m sin son tipo parrilla o de gas, y más de 0,50 m si son de otros tipos. Deben ser fácilmente accesibles y desmontables para su limpieza, tener una inclinación mayor que 45° y poseer  una  bandeja  de  recogida  de  grasas  que  conduzca  éstas  hasta  un  recipiente  cerrado  cuya  capacidad  debe  ser  menor  que 3 l.
- Los ventiladores cumplirán las especificaciones de la norma UNE-EN 12101-3: 2002 “Especificaciones para aireadores ex-tractores de humos y calor mecánicos.” y  tendrán una clasificación F400  90.

**Tabla 2.2. Condiciones de las zonas de riesgo especial integradas en edificios**

|Características:|Riesgo Bajo|Riesgo Medio|Riesgo Alto|
|:----|:----:|:----:|:------:|
|Resistencia al fuego de la estructura portante|R-90|R-120|R-180|
|Resistencia  al  fuego  de  las  paredes  y  techos  que  separan la zona del resto del edificio|EI-90|EI-120|EI-180|
|Vestíbulo  de  independencia  en  cada  comunicación  de la zona con el resto del edificio|-|SÍ|SÍ|
|Puertas de comunicación con el resto del edificio|EI<sub>2</sub>45-C5|2xEI<sub>2</sub>30-C5|2xEI<sub>2</sub>45-C5|
|Máximo recorrido hasta alguna salida del local|$\le$25M (6)|$\le$25M (6)|$\le$25M (6)|

<ins>NOTA 6:</ins>
Podrá aumentarse un 25% cuando la zona esté protegida con una Instalación automática de extinción


#### Sección SI-4, Instalaciones de Protección Contra Incendios

**Tabla 1.1. Dotacción de instalaciones de PCI**  
Necesitan INSTALACIÓN AUTOMÁTICA DE EXTINCIÓN las cocinas en:
- Uso Hospitalario o Residencial Público $\gt$ 20kW
- Cualquier otro Uso $\gt$ 50 kW

<a id="4"></a>

### Conclusiones

---
Cómo siempre: si crees que esta publicación se puede mejorar, encuentras alguna errata,
o piensas que algún contenido no expresa fielmente el contenido de algún Reglamento,
puedes enviarme tus comentarios a mi dirección de [e-mail][11].
</div>

*[CTE-DB-SI]: Código Técnico de la Edificación, Documento Básico Seguridad contra Incendios
*[DB-SI]: Documento Básico Seguridad contra Incendios


[^1]: Footnote

[1]:https://www.boe.es/eli/es/rd/2002/08/02/842/con
[2]:https://www.sodeca.com/es/software
[3]:https://www.sodeca.com/es/productos/cvt-p1000000076#prod
[4]:https://www.sodeca.com/es/productos/cjtht-p1000000048?cs=4&fil=50#prod

 
[11]:mailto:sesaba23@gmail.com


