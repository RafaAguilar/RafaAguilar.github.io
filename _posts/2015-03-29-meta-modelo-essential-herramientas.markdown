---
layout: post
title: "AE: Herramientas usadas para el Meta-Modelo de Essential Architecture"
author: rafa_aguilar
date: 2015-03-29 17:35:40
categories: entradas
comments: true
published: false
---

##Essential Architecture Manager

<div markdown="0"><a href="#" class="btn btn-danger">Alto!</a></div>
Se recomienda altamente haber leído **[esta entrada](/entradas/meta-modelo-de-essential-architecture/)** antes de seguir.
{: .notice}

El gestor de la arquitectura Essential es un conjunto the herramientas basdas en tecnologías **[libres][free]** enfocadas en soportar solamente prácticas de arquitectura empresarial aplicadas en el contexto de gestiones del negocio y de tecnologías de información tales como Gestión de Estrategias, entrega de soluciones, entrega de servicios, entre otros; haciendo énfasis en crear una herramienta de bajo mantenimiento (tanto en la arquitectura como en la plataforma), fácil de aprender y capaz de entregar resultados en semanas, en vez de meses.

Básicamente estas herramientas se pueden categorizar como la *parte modeladora* y la *parte visualizadora*, entre ellas existen una serie de componentes y relaciones que mostraremos en las siguientes imágenes

 - **Modeller y Viewer**
 
![](http://www.enterprise-architecture.org/images/stories/essential/eam_software_architecture.png)

 - **Roles y uso propuesto**
 
![](http://www.enterprise-architecture.org/images/stories/essential/em_high_level_context.png)
 
###Essential Modeller - Protégé

El modelador esta compuesto, en el núcleo, por una herramienta **[libre][free]** llamada [Protégé][protege] creada por la Universidad de Stanford y por una serie de extensiones que permiten capturar los datos y relaciones de los elementos tangibles y lógicos de la [Arquitectura Empresarial][AE] de una organización de manera simple y colaborativa. Su *meta-modelo*, a la fecha de escribir esta entrada, está en su versión 4.3.1 y verdad que es impresionante pensar en las horas/hombre que debe tener este producto.

![Capturas varias del modelador](http://www.enterprise-architecture.org/images/stories/essential/modeller_screenshots.png "Capturas del modelador")

<div markdown="0"><a href="#" class="btn btn-info">Info</a></div>
El modelador puede, opcionalmente, estar soportado por un repositorio centralizado almacenado en una base de dato relacional, como por ejemplo, Oracle DBMS&copy; o MySQL&copy;, para proveer una backend más robusto.
{: .notice}

###Essential Viewer - WebApp

El visor es una aplicación web que permite compartir y dividir en roles, las distintas [Vistas][vistas] que ofrece el [Meta-Modelo][mm] de *Essential Architecture*.  Esta se despliega en una plataforma de aplicaciones Java, como Apache Tomcat, que permita servir **Cien [Vistas][vistas]** dinamicamente creadas y poderosamente integradas en una fácil navegación para la visualización de las relaciones y análisis de las distintas capas compuestas en la [Arquitectura Empresarial][AE].


###Despliegue Estándar Multi-Usuario

Aunque se puede probar este conjunto de herramientas en una sola computadora personal (o versión *stand-alone*), para exprimir al máximo el provecho la [A.E.][AE], seguro se requerirá un conjunto de personas dedicadas al mantenimiento del repositorio, es por esto que se recomienda la instalación *Multi-Usuario*, que permitirá el trabajo en paralelo sobre el modelo.

En la siguiente imagen podrán visualizar un despliegue *estándar* de este tipo de instalación

![](/images/Essential_APP.svg) 

<div markdown="0"><a href="#" class="btn btn-info">Info</a></div>
_**nota**: los pasos a seguir de la instalación Multi-Usuario los puedes conseguir [aquí][multi] y los de la versión Stand-Alone los puedes conseguir [aqui][stand_alone]_ 
{: .notice}





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
[protege]:http:/protege.stanford.edu/
[vistas]:/entradas/meta-modelo-essential-workflow-y-vistas/#vistas
[mm]:/entradas/meta-modelo-de-essential-architecture/
[multi]:http://www.enterprise-architecture.org/documentation/doc-installation/148-installer-multi-user
[stand_alone]:http://www.enterprise-architecture.org/documentation/doc-installation/147-installer-stand-alone
{% include _toc.html %}