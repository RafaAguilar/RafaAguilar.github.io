---
layout: post
title:  "Archimate 2 MongoDB - En/On Python"
author: rafa_aguilar
date:   2015-04-12 11:35:40
categories: entradas
comments: true
---

#Versión en Español

![Experimental Logo][]

##Cuento Corto

El cuento corto es que [Archimate2MongoDB][a2m] es una herramienta libre desarrollada en Python v3.4 que permite analizar (*parse*) el [archivo del formato de intercambio Archimate][AFF] y colocarlo bajo una estructura *No-SQL* usando MongoDB como servidor.

##Cuento largo

El cuento *largo* es que esta iniciativa nace como una idea de oficina entre un colega (F. Rodríguez) debido a la necesidad de tener un motor de búsquedas del modelo que actualmente se está levantando allí, aunque usamos [Archi][archi] para modelar, excelente herramienta libre para esa tarea, no satisface todos los casos de usos en su desarrollo actual, es por esto que queremos devolver a la comunidad parte del beneficio que hemos obtenido, la idea base es crear una analizador avanzado sobre el cual podramos extraer información relevante rápidamente.

En la etapa actual tenemos como meta abarcar la fase 1 propuesta por el equipo de Open Group, donde podamos consultar cualquier elemento y obtener sus relaciones en cualquier nivel, filtrando los elementos de interés, además de crear posibilidades de edición en línea, vaciar desde MongoDB a XML, entre otras cosas.

La herramienta se encuentra desarrollada en Python v3.4, usando como motor MongoDB v3(como instalarlo [aquí][mongo]) y las librerías para Python PyMongo v3.0rc1

El repositorio está público en [Github : Archi2MongoDB][aca] 

###Hoja de ruta

Por los momentos nuestra *Hoja de ruta*(sin fechas) iría así: 

 - **v1** Soportar el análisis de la fase 1 del [archivo del formato de intercambio Archimate][AFF] y volcado en MongoDB.  
   - 1.1 Analizar Metadata.
   - 1.2 Analizar Capa Motivacional.
   - 1.3 Analizar Capa de Negocios.
   - 1.4 Analizar Capa de Aplicaciones.
   - 1.5 Analizar Capa de Infrastructura.
  
 - **v2** Crear servicios de búsqueda sobre los elementos:
   - 2.1 Relaciones filtradas por elementos.
   - 2.2 Nivel de *Peso* (idea en desarrollo).
   - 2.3 Dependencias entre los elementos.
   - 2.4 Usar propiedades para realizar el mapa de desarrollo propuesto.
   - 2.5 Usar propiedades para crear *brechas automáticamente*.
    
- **v3** Interfaz Gráfica (aún en fase conceptualización)

Por los momentos estamos en la versión 0 y si te interesa esta herramienta, no dudes en clonarla, mejorarla, probarla, traducirla, correr la voz y/o contacarte con nosotros, estaríamos agradecidos de cualquier apoyo ;).

Les debo el artículo sobre Archimate&copy;, en las próximas semanas saldrá junto al artículo de TOGAF&copy;.

_PD: el archivo `setup.py` puedes ignorarlo por los momentos, no se encuentra a tono._

#English Version

##Short History

The Short history is this,  [Archimate2MongoDB][a2m] is a Open Source Software developed in Python v3.4 that allows to parse the [ArchiMate® Model Exchange File Format][AFF] and dump the information into a *Non-SQL* structure using MongoDB as a background server.

##Long Hisotry
The long history goes like this, [Archimate2MongoDB][a2m] borns like an initiative from an office idea  between a colleague (F. Rodríguez) and me due to need a search engine to the Archimate model that we are constructing for the enterprise we work. We use [Archi][archi] to model the architecture, btw is an excellent Free Software tool, but does not satisfy all the use cases that we need in his actual version, that is why we want to give back to the community part of the benfit we have obtained from it, the idea is create an advanced analyzer that allows us extract relevant information real quick.

In the actual stage we have as a goal to support the Phase 1 of [ArchiMate® Model Exchange File Format][AFF], where we can consult any element and obtaing it's relationships at any leven, properties, description, and others, and filter those results by type or sub-types, besides allows to edit them online, reverse from MongoDB to XML, among other things.

###RoadMap

For now, our RoadMap(*without dates*) goes this way:

- **v1** Parsing [ArchiMate® Model Exchange File Format][AFF] Phase 1 support and dump on a MongoDB.
   - 1.1 Analyze Metadata.
   - 1.2 Analyze Motivational Layer.
   - 1.3 Analyze Business Layer.
   - 1.4 Analyze Applications Layer.
   - 1.5 Analyze Infrastrcuture Layer.
  
 - **v2** Create search services for the elements and :
   - 2.1 Filter relationships for type of element.
   - 2.2 Element weight index (an idea in desinging phase).
   - 2.3 Dependency between elements.
   - 2.4 Make use of properties to make the brochure of an possible roadmap(for a project).
   - 2.5 Make use of properties to make the gaps diagram automatically.
    
- **v3** Graphical User Interface (Still in conceptualization stage)

For now the tool is in v0, if you are interested on this tool, do not doubt on clone the repo, improve it, test it, translate it, spread the voice or (and) make contact with us, we will be grateful for anny kind of support ;).

_PD: the `setup.py` file should be ignore by now, it is not tune yet._

[a2m]:https://github.com/RafaAguilar/archi2mongodb
[AFF]:http://www.opengroup.org/subjectareas/enterprise/archimate/model-exchange-file-format
[archi]:www.archimatetool.com
[mongo]:http://rafaaguilar.github.io/entradas/mongo-30-en-rhel-5/
[aca]:https://github.com/RafaAguilar/archi2mongodb/
[a2mlogo]:/images/archi2mongo.png
{% include _toc.html %}
