---
title: RITE. Condiciones de Diseño
author: sesaba23
date: 2023-02-14
category: RITE
layout: post
published: true
---

## REGLAMENTO DE INSTALACIONES TÉRMICAS EN LOS EDIFICIOS. R.D. 1027/2007. 
## IT-1. Diseño y Dimensionado
*Publicado: {{ page.date | date_to_string}} \| Autor: {{ page.author }}*

---
> ##### AVISO
>
> Este post sólo pretende ser una guía-resumen de aplicación de la IT-1 del 
> Reglamento de Instalaciones Térmicas en los Edificios (RITE).
> Ten en cuenta que el texto Reglamentario es el único con validez legal.
> Puedes consultar [aquí][2] su contenido.
{: .block-warning }

<div markdown=1 style="text-align: justify">

#### Secuencia verificaciones (a incluir en el proyecto o memoria técnica):
1. Calidad térmica del ambiente (apartado 1.4.1).
2. Calidad de aire interior (apartado 1.4.2).
3. Calidad acústica (apartado 1.4.3.d).
4. Higiene (apartado 1.4.4).

#### IT 1.1.4.1 Calidad térmica del ambiente y valores para el dimensionado
Esta exigencia se considera satisfecha en el diseño y dimensionado de la instalación, 
si parámetros como la temperatura, humedad relativa, la velocidad media del aire, etc.
se mantienen dentro de de unos valores establecidos.

Los valores más representativos a tener en cuenta son: 

##### Temperatura operativa y Humedad Relativa (HR):
Hay que considerar las condiciones interiores de diseño de la tabla 1.4.1.1:

**Estación**|**Tª operativa ºC**|**HR %**
:---------- |:-------------------------: | :----:
Verano | 23...25 | 45...60
Invierno | 21...23 | 40...50

Lo anterior es válido para personas con actividad metabólica sedentaria de 1,2 met, 
con grado de vestimenta de 0,5 clo en verano y 1 clo en invierno y 
un PPD (porcentaje de personas insatisfechas) menor al 10 %. Asumimos también que
la velocidad del aire es baja (< 0,1 m/s).

Para actividades metabólicas y grados de vestimenta distintos ➡ UNE-EN ISO 7730.

Asimismo, si se trata de un centro de trabajo, también hay que remitirse a
[las disposiciones mínimas de seguridad y salud en los lugares de trabajo][1],
donde se indica, en relación a las condiciones ambientales (Anexo III):
- Trabajos sedentarios: 17 y 27ºC
- Trabajos ligeros: 14 y 25 ºC
- 30 $\le$  HR $\le$ 70% (Si hay riesgo electricidad estática HR $\le$ 50%)
- Corrientes de aire menores de:
    - Ambientes no calurosos: 0,25 m/s
    - Sedentarios en ambientes calurosos: 0,5 m/s
    - No sedentarios en ambientes calurosos: 0,75 m/s)

##### Velocidad media del aire EN ZONA OCUPADA (Tª seca del aire “t” entre 20ºC y 27ºC):
- Con difusión por mezcla, intensidad de turbulencia del 40% y 
PPD (Método Porcentaje de Personas insatisfechas) por corrientes de aire del 15%:

$$ V = {t \over 100} - 0,07 [m/s] $$

- Con difusión por desplazamiento, intensidad de turbulencia del 15% y 
PPD por corrientes de aire del 10%:

$$ V = {t \over 100} - 0,10 [m/s] $$

Para otros porcentajes de PPD (Porcentaje de personas insatisfechas) ➡ UNE EN ISO 7730 
y UNE-EN 13779.

#### IT 1.1.4.2 Calidad de aire interior
En viviendas, a locales habitables de su interior, almacenes de residuos y 
trasteros, y en aparcamientos y garajes: VÁLIDOS ➡ CTE HS 03.

En el RESTO ➡ Sistema de ventilación para aporte de caudal suficiente de aire exterior
➡ se puede hacer a través de ➡ UNE-EN 13779

##### Categorías del Calidad de Aire Interior (IDA):
- IDA1: Óptima (hospitales, clínicas, laboratorios, guarderías)
- IDA2: Buena (Oficinas, residencias, salas de lectura, museos, salas de tribunales, aulas de enseñanza, piscinas.
- IDA3: Media (Edificios comerciales, cines teatros, salones de actos, habitaciones de hoteles, restaurantes,    cafeterías, bares, salas de fiesta, gimnasios, deporte, salas de ordenadores)
- IDA4: Baja (aseos)

##### Caudal mínimo de aire exterior de ventilación:

Se puede seguir uno de los siguientes métodos:

<ins> A. Método indirecto de caudal de aire exterior por persona:</ins>

<p style="text-align: center;">Tabla 1.4.2.1 Caudales de aire exterior, 
en dm³/s (litros/s) por persona</p>

**Categoría**|**dm³/s por persona**
:----------: |:-------------------: 
IDA1 | 20 
IDA2 | 12,5 
IDA3 | 8 
IDA4 | 5 

Como observación, indicar que para IDA3, el cálculo se suele aproximar bastante
a 6 renovaciones/hora, valor típico que se consideraba hace años en este tipo de cálculos.

Hay que tener también en cuenta que Si se permite fumar, los caudales serán el doble. 
Si hay zonas delimitadas para fumadores, estas zonas consistirán en locales delimitados
por cerramientos estancos de aire y en depresión con respecto a locales contiguos. 

<ins> B. Método directo por calidad de aire percibido. Basado en informe CR 1752 (Método olfativo):</ins>

<p style="text-align: center;">Tabla 1.4.2.2 Calidad de aire percibido, en decipols</p>

**Categoría**|**dp**
:----------: |:-------------------: 
IDA1 | 0,8 
IDA2 | 1,2 
IDA3 | 2,0 
IDA4 | 3,0 

<ins> C. Método directo por concentración de CO2 en los locales</ins>: 

<p style="text-align: center;">Tabla 1.4.2.3 Concentración de CO2 en los locales</p>

**Categoría**|**pm (*)**
:----------: |:-------------------: 
IDA1 | 350 
IDA2 | 500 
IDA3 | 800 
IDA4 | 1.200 

*Concentración de CO2 (en partes por millón en volumen) por encima de la concentración en el aire exterior*

En bares, restaurantes y cafeterías se recomienda el método por dilución del apartado E.

<ins> D. Método indirecto de caudal de aire por unidad de superficie. Para espacios no dedicados a ocupación humana permanente: </ins>

<p style="text-align: center;">Tabla 1.4.2.4 Caudales de aire exterior por unidad 
de superficie de locales no dedicados a ocupación humana permanente</p>

**Categoría**|**dm³/(s*m²)**
:----------: |:-------------------: 
IDA1 | No aplicable 
IDA2 | 0,83 
IDA3 | 0,55 
IDA4 | 0,28 

<ins> E. Método de dilución. </ins>

Se aplica cuando en un local existan emisiones conocidas de materiales contaminantes 
específicos ➡ UNE EN 13779. Apartado 6.4.2.3.
En hospitales y clínicas son válidos los valores de la norma UNE EN 100713

##### Filtración del aire exterior mínimo de ventilación:

Clasificación en función de la Calidad de aire exterior (ODA):
- ODA1: aire puro que se ensucia sólo temporalmente (polen)
- ODA2: aire con concentraciones altas de partículas y gases contaminantes
- ODA3: aire con concentraciones muy altas de gases contaminantes o de partículas

<p style="text-align: center;">Tabla 1.4.2.5 Clases de filtración</p>
 
||**IDA1**|**IDA2**|**IDA3**|**IDA4**|
|:--- |:------: | :-----: |:--------: |:-----------: |
|ODA1 | F9 | F8 | F7 | F5 |
|ODA2 | F7 + F9 | F6 + F8 | F5 + F7 | F5 + F6 |
|ODA3 | F7 + GF*F9 | F7+GF+F9 | F5 + F7 | F5 + F6 |

<br>
Se emplearán prefiltros para mantener limpios los componentes de las unidades de
ventilación y tratamiento de aire. Se instalarán en la entrada de aire exterior 
a la unidad de tratamiento, y en la entrada del retorno.
Los aparatos de recuperación de calor deben estar siempre protegidos con una 
sección de filtros, cuya clase será la recomendada por el fabricante del recuperador; 
de no existir recomendación, serán como mínimo de clase F6.

##### Aire de extracción:

En función del uso del edificio o local, se clasifica en:
- AE1: bajo nivel de contaminación: aire que procede de los locales en los que 
las emisiones contaminantes proceden de materiales de construcción y decoración, 
además de personas.
No se incluye aire proveniente de locales donde se permite fumar.
Incluidos: oficinas, aulas, salas de reuniones, locales comerciales, 
espacios de uso público, escaleras y pasillos.

- AE2: moderado nivel de contaminación. Aires de locales con más contaminantes 
que la categoría AE1, no está permitido fumar.
Restaurantes, habitaciones de hoteles, vestuarios, aseos, cocinas domésticas 
(excepto campana extractora), bares, almacenes.

- AE3: Alto nivel de contaminación. Aire que procede de locales con producción 
de productos químicos, humedad, etc.

- AE4: Muy alto nivel de contaminación: locales que contienen sustancias olorosas
y contaminantes perjudiciales para la salud en concentraciones mayores que las 
permitidas en el aire anterioir de la zona ocupada.
Incluidos: extracción de campanas de humos, aparcamientos, locales de manejo 
de pinturas y disolventes, almacenamiento de residuos de cocina, 
locales con fumadores de uso continuo, laboratorios químicos.

Las condiciones que se deben cumplir son las siguientes:

- El caudal de extracción de locales de servicio será como mínimo de 2dm3/s por m2 de superficie en planta.
- Sólo el aire de categoría AE1, exento de humo del tabaco, puede ser retornado a los locales.
- El aire AE2 puede ser empleado solamente como transferencia de un local hacia locales de servicio, aseos y garajes.
- El aire AE3 y AE4 NO puede ser empleado como aire de recirculación o de transferencia.
- Cuando se mezclan aires de distintas categorías se entiende que es la más desfavorable.
- Si las extracciones se realizan de manera independiente, la expulsión hacia el exterior 
del aire de las categorías AE3 y AE4 no puede ser común a la expulsión del aire de las 
categorías AE1 y AE2, para evitar la posibilidad de contaminación cruzada

#### IT 1.-1.4.3 Exigencia de higiene

Hay que tener en cuenta principalmente lo siguiente:
- Preparación de agua caliente para usos sanitarios ➡ Según normativa higiénico-sanitaria.
- Apertura de servicio para limpieza de conductos de aire:
    - Las redes de conductos deben estar equipadas de aperturas de servicio para permitir limpieza y desinfección.
    - Elementos de conductos deben ser desmontables
    - Los falsos techos deben tener registros de inspección

#### IT 1.-1.4.4 Exigencia de calidad del ambiente acústico: 

Unicamente se dice que las instalaciones térmicas de los edificios deben cumplir 
la exigencia del documento [**DB-HR Protección frente al ruido del Código Técnico de la Edificación**][3], 
que les afecten.

#### IT 1.2 EXIGENCIA DE EFICIENCIA ENERGÉTICA
##### IT 1.-2.4.5.2 Recuperación de calor del aire de extracción
Lo más destacable de este apartado es que los sistemas de climatización de los edificios
en los que el caudal de aire expulsado al exterior, por medios mecánicos, sea superior 
a **0,28 m3/s**, se recuperará la energía del aire expulsado

*Un apreciación: Durante años el valor del caudal de aire expulsado fue de 0,5 m³/s.*
*El 24 de marzo de 2021, se modificó el reglamento para reducir dicho valor*

#### IT 1.-2.4.6.4 Climatización de espacios abiertos.
La climatización de espacios abiertos sólo podrá realizarse mediante la utilización 
de energías renovables o residuales. No podrá utilizarse energía convencional para 
la generación de calor y frío destinado a la climatización de estos espacios.


##### Varios:
Para terminar este Post, como curiosidad, destacar que a finales de 2022, como
consecuencia de la escasez de gas natural debido a la guerra de Ucrania, 
y para intentar reducir el consumo energético, según compromiso adquirido con la UE
se introdujo el siguiente texto en la **IT 3.8.4** relativo a la apertura de puertas:
Los edificios y locales con acceso desde la calle dispondrán de un sistema de cierre 
de puertas adecuado, el cual podrá consistir en un sencillo brazo de cierre automático 
de las puertas, con el fin de impedir que éstas permanezcan abiertas permanentemente, 
con el consiguiente despilfarro energético por las pérdidas de energía al exterior, 
cuando para ello se requiera consumo de energía convencional para la generación 
de calor y frío por parte de los sistemas de calefacción y refrigeración.

---
Si crees que esta publicación se puede mejorar, encuentras alguna errata,
o piensas que algún contenido no expresa fielmente el contenido del RITE,
puedes enviarme tus comentarios a mi dirección de [e-mail][4].
</div>

*[RITE]: Reglamento de Instalaciones Térmicas en Edificios

[1]:https://www.boe.es/buscar/act.php?id=BOE-A-1997-8669
[2]:https://www.boe.es/buscar/act.php?id=BOE-A-2007-15820&p=20220802&tn=1#it1-2
[3]:https://www.codigotecnico.org/pdf/Documentos/HR/DBHR.pdf
[4]:mailto:sesaba23@gmail.com