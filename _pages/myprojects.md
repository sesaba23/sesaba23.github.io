---
title: Mis Proyectos
author: sesaba23
date: 10/02/2023
category: sesaba
layout: post
---
---

<div markdown=1 style="text-align: justify">

Estos son los Proyectos más relevantes que he desarrollado en orden cronológico:

Web Scraping del BOE para Oposiciones Públicas:
: Aplicación sobre línea de comandos que permite hacer **web scraping** del 
Boletín Oficial del Estado (BOE) para extraer información sobre convocatorias de oposiciones 
publicadas por las Administraciones Públicas en el BOE, especialmente la Administración del Estado
y las Administraciones Locales. 
Los resultados se almacenan en un archivo Excel y se pueden filtrar por fechas y patrones de búsqueda.
Es una gran herramienta para aquellas personas que estén preparando oposiciones ya que también
permite buscar convocatorias en función del tipo de plaza en un rango de fechas especificado,
permitiendo ahorrar una gran cantidad de tiempo.
Aunque actualmente estoy implementando nuevas mejoras y funcionalidades, es
totalmente funcional. Poco a poco iré publicando nuevas mejoras.
Puedes descargarla en mi [Github personal][18] y contribuir con el proyecto
ya que es de código abierto.

![imagen]({{ site.url }}/assets/images/web-scraping-resultados.jpg) 

![imagen]({{ site.url }}/assets/images/web-scraping-map.jpg) 


Proyecto Web con Django:
: Actualmente estoy aprendiendo [Python][15] y desarrollo web con [Django][16]. Para ello,
he implementado una página web personal típica con operaciones CRUD, base de datos
con [Postgresql][14], un sistema de acceso premium, blog con comentarios y tienda
para venta de productos. El código fuente esta en mi [GitHub][12]. La aplicación 
web está dockerizada, por lo que puedes probarla muy facilmente si instalas [Docker][13].


Herramienta para la gestión del inventario de elementos viales:
: Cuando me incorporé a un nuevo puesto de trabajo relacionado con proyectos y 
movilidad urbana, adapté mi herramienta de asistencia de proyectos de alumbrado público
de manera que permitiese inventariar cualquier clase de mobiliario urbano, especialmente
señalización vial vertical inteligente. Permite conformar un inventario y planos
en formato AutoCAD de manera que facilite la gestión del mantenimiento de este tipo
de instalaciones. También agiliza la redacción de proyectos. Además, he creado 
un módulo que permite calcular el presupuesto desglosado de la instalacióm en un click, 
y que está desarrollado en Django, utilizando las librerias [Pandas][10] y [Openpyxl][11].
Esta herramienta está integrada en mi Proyecto Web y puedes acceder a ella si estás
registrado.
: Si crees que te puede ser util y quieres que la 
adapte a tu empresa o necesidades personales, puedes [contactar conmigo][9].  

![imagen]({{ site.url }}/assets/images/svv-proyecto.jpeg) 

Herramientas de asistencia para proyectos de eficiencia energética de A.P.:
: En 2018, cambié de trabajo pasando a ser Director de Proyectos de eficiencia energética.
El caso es que me asignaron la redacción de decenas de proyectos de eficiencia de
alumbrado público y sus direcciones técnicas con un equipo de personas exiguo.
Desde el primer momento, me di cuenta de que siguiendo el método clásico era imposible.
Uno de mis jefes llevaba años desarrollando una herramienta similar
y me dio la idea. Así fue como llevé a cabo este proyecto que permite automatizar
la mayoría de tareas para la redacción de este tipo de proyectos. Está desarrollada
en VBA haciendo uso de su libreria para Autocad, permitiendo también conformar
todos los cálculos, justificar la inversión necesaria para ejecutarla, los planos
de la instalación y el presupuesto de Ejecución Material.
Esta aplicación me sirvió como base para redactar el TFM de mi Máster en Ingeniería
Industrial y que fue propuesto para Matrícula de Honor en la promoción de 2022.
: Aquí puedes descargar la [memoria]({{ site.url }}/assets/resources/TFM_MUII.pdf). 
Al igual que antes, si estás interesado en conocer en profundidad
sus funcionalidades puedes [contactar][9] conmigo. También si quieres hacer uso 
de ella o necesitas que la adapte a tus necesidades.

Ruby on Rails y Desarrollo Ágil:
: Hace unos años me interesaba aprender sobre desarrollo ágil e hice un par de
cursos en la plataforma [edx][17] impartidos por la Universidad de [Berkeley][6] (California).
Gracias a estos cursos pude participar en un *Mooquita Challenger* relacionado con la IA
dirigido por un investigador de Google, [Praveen Paritosh][7], en un equipo
con participantes de varios paises. En mi [perfil de GitHub][8] puedes ver el código.

Gestitime:
: Gestitime es una aplicación pensada para gestionar el tiempo a la hora de hacer 
cualquier tarea. En aquella época tenía que preparar una presentación para un 
proceso selectivo en un tiempo determinado.
La exposición era pública y el lugar donde estaba prevista no contaba con el
típico reloj colgado en la pared; mirar continuamente mi reloj de muñeca o el móvil 
estaba descartado.
Se me ocurrio que tenía que existir alguna aplicación para el móvil que me
permitiese, de alguna manera, establecer un tiempo determinado con avisos
prestablecidos y que, mediante vibraciones, llevándolo en el bolsillo, me
facilitase tener un cierto control del tiempo transcurrido. El caso es que no la encontré
y así surgió la idea de desarrollar Gestitime.
: La aplicación está publicada en la Tienda de Aplicaciones de Google. [Aquí][4] 
puedes descargarla e instarla desde tu movíl o tablet. También puedes ver su 
código [fuente][5].
{:refdef: style="text-align: center;"}
![imagen]({{ site.url }}/assets/images/gestitime.jpeg)
{:refdef}

Gestiaguas v2:
: Mis primeros pinitos con **Java** sirvieron para actualizar Gestiaguas v1.
Migré la base de datos a MySQL, mejorando y ampliando su estructura y renové
el interfaz de la aplicación utilizando Java Swing. Además, desarrollé una nueva versión
para realizar las lecturas de los contadores de agua en Android, mucho más completa
y funcional. Puedes ver el código fuente en mi [Bitbucket][3].

Gestiaguas v1
: Como ves tenía un nombre muy original. La creé en 2005 y fue mi primer contacto
con el mundo de la programación. Se centraba en una herramienta
que permitía la gestión de las lecturas de contadores de agua domiciliaria e 
industrial de un municipio de unos 10.000 habitantes.
: Se utilizó de manera eficaz durante muchos años y básicamente se componía de
una base de datos *Access*, relativamente compleja. La Lectura se hacía
mediante PDAs programadas con *Visual CE* que permitián al lector gestionar
rutas, actualizar facilmente los datos de los puntos de consumo e introducir las lecturas
de agua de los contadores.
: Gestiaguas sirvió como base para realizar mi trabajo final de carrera de
Ingeniería Electrónica y fue calificado con Matrícula de Honor.
Puedes descargar una copia del trabajo en el siguiente 
[enlace]({{ site.url }}/assets/resources/TFM_IE.pdf).
</div>



[3]:https://sesaba23@bitbucket.org/sesaba23/gestiaguas.git
[4]:https://play.google.com/store/apps/details?id=com.ssb.gestitime&hl=es&gl=US
[5]:https://bitbucket.org/sesaba23/gestitime/src/master/
[6]:https://www.edx.org/course/introduction_to_agile_software_development
[7]:https://www.linkedin.com/in/pkparitosh
[8]:https://github.com/sesaba23/iccg-team-red
[9]:mailto:sesaba23@gmail.com
[10]:https://pandas.pydata.org/
[11]:https://openpyxl.readthedocs.io/en/stable/
[12]:https://github.com/sesaba23/myweb
[13]:https://docs.docker.com/get-started/overview/
[14]:https://www.postgresql.org/
[15]:https://www.python.org/
[16]:https://www.djangoproject.com/
[17]:https://www.edx.org/es
[18]:https://github.com/sesaba23/ope-boe-scraping