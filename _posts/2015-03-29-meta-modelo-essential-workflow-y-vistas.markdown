---
layout: post
title: "AE: Flujo de trabajo propuesto para Essential Architecture"
author: rafa_aguilar
date: 2015-03-29 11:35:40
categories: entradas
comments: true
published: false
---

###Flujo de trabajo

<div markdown="0"><a href="#" class="btn btn-danger">Alto!</a></div>
Se recomienda altamente haber leído **[esta entrada](/meta-modelo-essential-herramientas/) y [esta otra](/entradas/meta-modelo-essential-workflow-y-vistas/)** antes de seguir.
{: .notice}

Debido a lo complejo que puede ser implementar la [A.E.][AE] desde nad ao cero, se propone un flujo de trabajo derivado del propuesto por los chicos de [EAS][eas], es sólo una humilde propuesta de como una organización podría abordar el crear su arquitectura base o actual siguiendo estos cuantro (4) pasos, además de los referenciados en cada uno.

#### **1.** **Análisis Previo**

Aunque con el meta-modelo se facilita un poco poder modelar(valga la redundancia) la organización en sus elementos, iniciar el análisis a la vez que se toma la estrategia *AE*[^1] es bastante complejo y puede retrasar o detener por completo este proceso, y no es lo que se desea, por eso se propone conocer lo más posible los principios o lineamientos, estructura orgánica, formatos o documentos, normas o reglamentos y principales funciones y entorno(cadena de valor de alto nivel) de la organización antes de iniciar el modelado. \\
Para esto se pueden usar herramientas variadas como [A3][a3], [Diagramas BPMN][bpmn], encuestas, entre otras técnicas de levantamiento de información que te puedan aportar los datos necesarios para conocer las interacciones de alto(o mediano) nivel de los principales procesos de la organización.

#### **2.** **Cadena de valor**
El meta-modelo es altamente abstracto, lo recomendado, entonces, es por comenzar por la zona más concreta que es la capa de negocios, hay una relación directa entre procesos medulares y lo que conoceremos como *[Capacidades][caps]* en el mundo de [TOGAF][togaf]&copy;, las interacciones y secuencia entre ellas y los [Actores y Roles][actors_roles] involucradas en las actividades de la empresa.\\
Registramos todas los elementos arriba mencionados procurando crear sólo los objetos con las relaciones detectadas y previamente analizadas, es decir, registrar lo previsto hasta el momento, ya que cuando estemos modelando seguramente surgirán nuevas relaciones o ideas de detalles que podrían desviarnos del objetivo principal que es tener un modelo a alto nivel.\\
Podemos observar acá los distintos elementos y relaciones de la capa de negocios:  ![](http://www.enterprise-architecture.org/images/stories/essential/tutorials/layers/business_layer_overview.png)
_**+info:** Para más información de como abordar la capa de negocio podemos ver este **[Tutorial][tut_bus]** que profundiza en el tema._

<div markdown="0"><a href="#" class="btn btn-info">Nota</a></div>

Por los momentos no hace falta identificar todas las actividades de soporte, a medida que estan vayan siendo claras durante todo el modelado podemos irlas agregando.
{: .notice}

#### **3.** **Estandarización de la información**
De todos los elementos modelados en la capa de negocios emergerán documentos, funciones, roles, sistemas, entre otros, que consideraremos elementos de información(de ahora en adelente *ei*, y para cada cual tendremos que tener _**definiciones**_, _**interacciones** y **representaciones**_ y _**almacenes**_.\\
Las ***definiciones*** podemos agruparlas en la categoría de *ei* conceptuales.  Esta podrá usarse como una especie de glosarios de términos propios del negocio, donde además podremos nutrirlos con relaciones como a que otros *ei* es relevante son, o enlaces de referencia externos que nos ayuden a definir el concepto. También se pueden definir objetivos y lineamientos(*[principios][principles]*) que gobernarán el _como se hace_ o  _como debemos_ manipular o almacenar los *ei*.\\
Las ***interacciones*** y ***representaciones*** podemos agruparlas en *vistas lógicas* que nos permitan visualizar las relaciones o conceptos sin necesidad de tener que capturar cada atributo de los *ei* identificando la tecnología usada, a nivel lógico, para el almacenamiento de cada una, es decir si usaremos alguna notación o una base de datos relacional, orientada a documentos, etc.\\
Los ***almacenes*** no son más que cuales estructuras físicas soportan o almacenan los *ei*, luego sabremos la importancia de conocerlas y tenerlas modeladas.\\
Podemos observar acá los distintos elementos y relaciones de la capa de información:  ![](http://www.enterprise-architecture.org/images/stories/essential/tutorials/layers/information_layer_overview.png)

#### **4.** **Mapa de elementos y relaciones virtuales**
Las relaciones de los elementos del negocio y de información identificados en las secciones anteriores, no siempre son tangibles, de hecho, en una organización moderna, la mayoría se interconectan virtualmente vía electrónica a través de sistemas, de nuevo, físicos y tangibles, mediante sistemas de información automatizados.  Esto añade mayor complejidad a las relaciones, sin embargo conocer estas últimas son de suma importancia, ya que es como el sistema nervioso de un organismo, si vemos el resto como un cuerpo. 
    + Para determinar estas relaciones se sugeriría empezar por detallar más las capacidades detectadas en **1** generando diagramas de procesos (_BPM_) e identificando los sistemas y servicios que usan para las actividades profundizadas en dicho análisis.  De esta manera se engranará, en un primer nivel, la capa de negocios con la capa de aplicaciones, permitiendo modelar las relaciones virtuales y las interdependencia entre los sistemas y procesos.
    + Luego de identificar los sistemas y los servicios y funciones que estos proveen, podemos generar las relaciones sobre las dependencias que existen entre aplicaciones y proveedores de aplicaciones, un ejemplo sería **[Essential Viewer][ea_viewer]** y __Apache Web Sever__, la aplicación y el proveedor respectivamente.
    + Por último la _capa de infraesctura_ no es más que la representación físico de donde se ejecutan, almacenan y procesan los distintos servicios provistos en la _capa de aplicaciones_, versiones de software base (como Sistema Operativo...) e información de capacidad de los equipos destinados a ellos (como cantidad de memoria o de espacio en discos), de manera que con estas relaciones cerramos las relaciones que llevamos desde lo concreto, el **negocio**, a lo asbtracto, **servicios y funciones de aplicaciones** y de vuelta a lo concreto con la **plataforma física**.    \\
Podemos observar acá los distintos elementos y relaciones de la capa de aplicaciones:  ![](http://www.enterprise-architecture.org/images/stories/essential/tutorials/layers/application_layer_overview.png)\\
Podemos observar acá los distintos elementos y relaciones de la capa de infraestructura:  ![](http://www.enterprise-architecture.org/images/stories/essential/tutorials/layers/technology_layer_overview.png)

<div markdown="0"><a href="#" class="btn btn-info">Info</a></div>    
_Para más información de como abordar la capa de aplicaciones e infraestructura podemos ver estos **[Tutorial C. Aplicaciones][tut_app]** y **[Tutorial C. Infraestructura][tut_inf]** que profundizan los temas._
{: .notice}

###Vistas

Parte de lo que podemos esperar acá lo podemos ver reflejado en las siguientes vistas, que no son mas que un sub-conjunto de todas las incluídas en el [Catálogo de vistas][catalogue_view].

 - **Modelado de Procesos de Negocios**
![BPM](http://www.enterprise-architecture.org/images/stories/essential/viewer3_screenshots/04%20-%20business%20process%20model.png)
 
 - **Catálogo de Conceptos de información**
![Catalogo de conceptos](http://www.enterprise-architecture.org/images/stories/essential/viewer3_screenshots/12%20-%20information%20catalogue%20by%20concept.png)

 - **Modelo de dependencia de Aplicaciones**
![Dependencia de Aplicaciones](http://www.enterprise-architecture.org/images/stories/essential/viewer3_screenshots/03%20-%20application%20dependencies%20model.png)

 - **Matriz de Permisología (roles)**
![Data-to-Role Matrix](http://www.enterprise-architecture.org/images/stories/essential/viewer3_screenshots/11%20-%20data%20security%20model.png)

 - **Modelo de referencia de Tecnologías**
![TI Reference Model](http://www.enterprise-architecture.org/images/stories/essential/viewer3_screenshots/07%20-%20technology%20reference%20model.png)



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
{% include _toc.html %}
