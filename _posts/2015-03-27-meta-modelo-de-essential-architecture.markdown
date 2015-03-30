---
layout: post
title: "AE: El proyecto 'Essential'"
author: rafa_aguilar
date: 2015-03-27 11:35:40
categories: entradas
comments: true
published: true
---

#El proyecto

El proyecto *Essential* nace de una inicativa promovida por [Enterprise Architecture Solutions Ltd][eas], el cual busca impulsar que las empresas y organizaciones, de cualquier escala saquen, el mejor provecho del valor agregado que ofrece la [Arquitectura Empresarial][AE] disminuyendo las dificultades y aportando herramientas **[libres][free]** que briden simpleza sin ir en detrimento de la productividad.  Dejemos que ellos mismos lo expliquen con sus palabras:

>The goal of The Essential Project is to promote the value that enterprise architecture can bring to organisations of all sizes and experience by lowering barriers to entry with a free, simple, productive and, most importantly, effective set of supporting tools.<sup markdown="1">[fuente]</sup>

El proyecto también cuenta con una excelente [comunidad][eas_comm] que lo respalda y que motoriza el hecho que se mantendrá libre tanto sus herramientas y base también lo son, otorgando así proyección a cualquier organización que se determine usarla.

El principal objetivo de estos chicos es intentar desmontar la *[A.E.][AE]* de la burbuja o la *torre de marfil* donde se cree que es un estudio muy avanzado y desapegado a la realidad, donde el fin es entender abstractamente los elementos e interrelaciones en una organización, cuando en realidad la *AE*[AE] ofrece gigantescas ventajas competitivas con apenas semanas de esfuerzo.

<div markdown="0"><a href="#" class="btn btn-info">Recomendación</a></div>

_**Prefereiblemente** se requiere tener conocimientos, al menos básicos, sobre modelado **[UML][uml]** debido a que en la metodología propuesta se usan muchos conceptos **core** y conceptos análogos de esta notación._
{: .notice}

Expliquemos un poco de que va la propuesta del proyecto _Essential_:

##Essential Meta-Model

El Meta-Mode
lo _Essential_ ofrece todo un marco de trabajo informal, aunque los chicos de *Essential* lo propongan como guías de mejores prácticas y tips de ayudas, que se basa en [TOGAF][togaf]&copy;,  marco de trabajo formal desarrollado por [OpenGroup][opengroup]. 

Este modelo ofrece elementos, relaciones, enlaces, descripciones y identificadores para cada capa propuesta en [TOGAF][togaf]&copy;, para ahondar más en esta información puedes visitar la [excelente documentación][mm-doc] que ofrecen en su página los chicos del proyecto.

Como las imágenes valen más que mil palabras, acá un diagrama conceptual del modelo:

![](http://www.enterprise-architecture.org/images/stories/essential/eamm_scope.png)

<div markdown="0"><a href="#" class="btn btn-warning">Importante</a></div>

_La intensión de esta entrada no va a ser dar detalle de cada una de las capas o de lo que ofrece el meta-modelo, sino de ofrecer una opinión de las ventajas y deventajas para una organización al abordar la **[A.E.][AE]** como estrategia de análisis de la situación actual o futura de si misma usando las herramientas y flujo de trabajo de Essential.\\
\\
Si desea profundizar puede leer el artículo de **[las herramientas][ea_toolset]** usadas  y el del **[flujo de trabajo propuesto][workflow]**._
{: .notice}

###Resumen

Para la *evaluación*, o mejor dicho *apreciación subjetiva*, sólo tomaré en cuenta el [flujo de trabajo][workflow] y [[Herramientas][ea_toolset] propuesto por los chicos de [EAS][eas] dejando *por fuera* los beneficios que trae consigo la [A.E.][AE] como estrategia de una organización.

Empezaré por un listado de las ventajas y desventajas:

####Ventajas

 - Basada en un metodología probada y exhaustiva como lo es [TOGAF][togaf]&copy;
 - Completamente apegada a las directrices del estándar de [TOGAF][togaf]&copy; en su versión 9
 - Al estar sus herramientas basadas [Software Libre][free] la sostenibilidad está garantizada 
 - Excelente comunidad y documentación sobre el manejo de sus herramientas
 - Repositorio centralizado para trabajo colaborativo
 - Cien (100) reportes listos *out-of-the-box* separados por roles
 - Herramienta para importar datos de fuentes externas, excelente migración garantizada
 - Todos los Elementos propuestos por [TOGAF][togaf]&copy; ya creados en el repositorio (clases y relaciones) ya creadas al inicio
 - 

####Desventajas

 - Excesivamente exhaustivo, para cada elemento de [TOGAF][togaf]&copy; existe una entrada en el formulario de cada una de las posibles relaciones, esto hace que ingresar la información de un elemento se dificulte
 - Baja flexibilidad *out-of-the-box*, para gozar del beneficio de todas las vistas pre-creadas, se debe trabajar al estilo *essential-way*, sino probablemente se verán muchas vistas vacías
 - Aunque se pueden crear reportes nuevos y usar como plantilla los existentes, es un formato que embebe notación HTML, XML, SVG y código JavaScript (cuidado si no se me escapa algo), y todo en un solo archivo.. resulta bastante tedioso modificar uno o intentar hacer alguno desde cero para alguien no familiarizado.
 - La diagramación BPMN y de la Cadena de Valor deja mucho que desear
 - Los formularios no son pensados, *IMHO*, para diagramar o modelar desde un comienzo en ellas, están más enfocadas en el "vaciado" de información en el repositorio a través de los mismos un análisis ya realizado de la [A.E.][AE] actual.
 - El Meta-Modelo no es extensible facilmente (al menos no conseguí como hacerlo en este análisis)
 - Conseguir elementos (o clases) resulta bastante complejo no es intuitiva en todos los casos.
 
####Conclusión

Seguramente se escapan algunas ventajas o desventajas, y claramente esta lleno de subjetividad, sin embargo debo decir que la herramienta es tremendamente potente, ofrece un valor agregado inmenso (aparte del que ofrece la [A.E.][AE] en si, y simplifica un poco el trabajo de modelar la arquitectura base o actual de una organización, sin embargo, creo que el objetivo trazado de entregar resultados en *días o semanas* como dicen los chicos de [EAS][eas] no aplica en todos los casos, y en organizaciones de medianas a grandes puede resultar bastante complejo y de gran esfuerzo, aunque no digo que no se merezca invertir este esfuerzo.

Para una organización pequeña o naciente me parece una gran iniciativa en la cual si se cumplen los objetivos de entregar resultados a corto plazo y permite alta escalabilidad como para que pueda mantenerse, incluso hasta desarrollarse como una gran organización.  Ahora, para empresas u organizaciones de medianas a grandes ya cosntituidas y no cercanas a la [A.E.][AE] puede ser un *escalón* mayor de complejidad el crear y mantener, en un inicio, la arquitectura base.



[fuente]: http://www.enterprise-architecture.org/about/mission
[eas]: http://www.enterprise-architecture.org/component/weblinks/weblink/39-eas/6-eas-home
[AE]: /entradas/arquitectura-empresarial/
[free]: http://es.wikipedia.org/wiki/Software_libre
[eas_comm]: http://www.enterprise-architecture.org/community
[^1]: Arquitectura Empresarial ver [más][AE]
[opengroup]:https://www.opengroup.org/togaf/
[togaf]:/en-construccion.html
[uml]:/en-construccion.html
[caps]:/en-construccion.html
[a3]:/en-construccion.html
[principles]:/en-construccion.html
[actors_roles]:/en-construccion.html
[bpmn]:/en-construccion.html
[mm-doc]:http://www.enterprise-architecture.org/documentation/doc-meta-model
[tut_bus]:http://www.enterprise-architecture.org/business-architecture-tutorials
[tut_app]:http://www.enterprise-architecture.org/application-architecture-tutorials/57-application-architecture-overview
[tut_inf]:http://www.enterprise-architecture.org/techology-architecture-tutorials/58-techology-architecture-overview
[ea_viewer]:/en-construccion.html
[workflow]:/entradas/meta-modelo-essential-workflow-y-vistas/
[ea_toolset]:/entradas/meta-modelo-essential-herramientas/
{% include _toc.html %}
