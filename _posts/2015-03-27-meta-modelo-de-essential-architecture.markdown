---
layout: post
title: "AE: El proyecto *Essential*"
author: rafa_aguilar
date: 2015-03-27 11:35:40
categories: entradas
comments: true
published: true
---

#El proyecto *Essential*

El proyecto *Essential* nace de una inicativa promovida por [Enterprise Architecture Solutions Ltd][eas], el cual busca impulsar que las empresas y organizaciones, de cualquier escala saquen, el mejor provecho del valor agregado que ofrece la [Arquitectura Empresarial][AE] disminuyendo las dificultades y aportando herramientas **[libres][free]** que briden simpleza sin ir en detrimento de la productividad.  Dejemos que ellos mismos lo expliquen con sus palabras:

>The goal of The Essential Project is to promote the value that enterprise architecture can bring to organisations of all sizes and experience by lowering barriers to entry with a free, simple, productive and, most importantly, effective set of supporting tools.<sup markdown="1">[fuente]</sup>

El proyecto también cuenta con una excelente [comunidad][eas_comm] que lo respalda y que motoriza el hecho que se mantendrá libre tanto sus herramientas y base también lo son, otorgando así proyección a cualquier organización que se determine usarla.

El principal objetivo de estos chicos es intentar desmontar la *AE*[^1] de la burbuja o la *torre de marfil* donde se cree que es un estudio muy avanzado y desapegado a la realidad, donde el fin es entender abstractamente los elementos e interrelaciones en una organización, cuando en realidad la *AE*[^1] ofrece gigantescas ventajas competitivas con apenas semanas de esfuerzo.

<div markdown="0"><a href="#" class="btn btn-info">Advertencia</a></div>

_**Prefereiblemente** se requiere tener conocimientos, al menos básicos, sobre modelado **[UML][uml]** debido a que en la metodología propuesta se usan muchos conceptos **core** y conceptos análogos de esta notación ._
{: .notice}

Expliquemos un poco de que va la propuesta del proyecto _Essential_:

##Essential Meta-Model

El Meta-Modelo _Essential_ ofrece todo un marco de trabajo informal, aunque los chicos de *Essential* lo propongan como guías de mejores prácticas y tips de ayudas, que se basa en [TOGAF][togaf]&copy,  marco de trabajo formal desarrollado por [OpenGroup][opengroup]. 

Este modelo ofrece elementos, relaciones, enlaces, descripciones y identificadores para cada capa propuesta en [Togaf][togaf]&copy, para ahondar más en esta información puedes visitar la [excelente documentación][mm-doc] que ofrecen en su página los chicos del proyecto.

<div markdown="0"><a href="#" class="btn btn-warning">Importante</a></div>

_La intensión de esta entrada no va a ser dar detalle de cada una de las capas o de lo que ofrece el meta-modelo, sino de ofrecer una visión sobre como podría una organización abordar el uso de la **AE**[^1] como estrategia de análisis de la situación actual o furura de si misma usándolo._
{: .notice}

<!-- Artículo 2 -->

###Flujo de trabajo

- **1.** **Análisis Previo**: Aunque con el meta-modelo se facilita un poco poder modelar(valga la redundancia) la organización en sus elementos, iniciar el análisis a la vez que se toma la estrategia *AE*[^1] es bastante complejo y puede retrasar o detener por completo este proceso, y no es lo que se desea, por eso se propone conocer lo más posible los principios o lineamientos, estructura orgánica, formatos o documentos, normas o reglamentos y principales funciones y entorno(cadena de valor de alto nivel) de la organización antes de iniciar el modelado. \\
Para esto se pueden usar herramientas variadas como [A3][a3], [Diagramas BPMN][bpmn], encuestas, entre otras técnicas de levantamiento de información que te puedan aportar los datos necesarios para conocer las interacciones de alto(o mediano) nivel de los principales procesos de la organización.

- **2** **Cadena de valor**: El meta-modelo es altamente abstracto, lo recomendado, entonces, es por comenzar por la zona más concreta que es la capa de negocios, hay una relación directa entre procesos medulares y lo que conoceremos como *[Capacidades][caps]* en el mundo de [TOGAF][togaf]&copy;, las interacciones y secuencia entre ellas y los [Actores y Roles][actors_roles] involucradas en las actividades de la empresa.\\
Registramos todas los elementos arriba mencionados procurando crear sólo los objetos con las relaciones detectadas y previamente analizadas, es decir, registrar lo previsto hasta el momento, ya que cuando estemos modelando seguramente surgirán nuevas relaciones o ideas de detalles que podrían desviarnos del objetivo principal que es tener un modelo a alto nivel.\\
_**+info:*** Para más información de como abordar la capa de negocio podemos ver este [Tutorial][tut_bus] que profundiza en el tema._

<div markdown="0"><a href="#" class="btn btn-info">Nota</a></div>

Por los momentos no hace falta identificar todas las actividades de soporte, a medida que estan vayan siendo claras durante todo el modelado podemos irlas agregando.
{: .notice}

- **3.** **Estandarización de la información**: De todos los elementos modelados en la capa de negocios emergerán documentos, funciones, roles, sistemas, entre otros, que consideraremos elementos de información(de ahora en adelente *ei*, y para cada cual tendremos que tener _**definiciones**_, _**interacciones** y **representaciones**_ y _**almacenes**_.\\
Las ***definiciones*** podemos agruparlas en la categoría de *ei* conceptuales.  Esta podrá usarse como una especie de glosarios de términos propios del negocio, donde además podremos nutrirlos con relaciones como a que otros *ei* es relevante son, o enlaces de referencia externos que nos ayuden a definir el concepto. También se pueden definir objetivos y lineamientos(*[principios][principles]*) que gobernarán el _como se hace_ o  _como debemos_ manipular o almacenar los *ei*.\\
Las ***interacciones*** y ***representaciones*** podemos agruparlas en *vistas lógicas* que nos permitan visualizar las relaciones o conceptos sin necesidad de tener que capturar cada atributo de los *ei* identificando la tecnología usada, a nivel lógico, para el almacenamiento de cada una, es decir si usaremos alguna notación o una base de datos relacional, orientada a documentos, etc.\\
Los ***almacenes*** no son más que cuales estructuras físicas soportan o almacenan los *ei*, luego sabremos la importancia de conocerlas y tenerlas modeladas.

- **4.** ****

###Vistas

<!-- Artículo 3 -->
##Essential Architecture Manager
###Essential Modeler - Protégé
###Essential Viewer - WebApp

<!-- Artículo Original -->
###Ventajas
###Desventajas
###Conclusión

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
{% include _toc.html %}
