---
layout: post
title:  "Arquitectura Empresarial"
author: rafa_aguilar
date:  2015-03-25 12:35:40
categories: entradas
comments: true
---

{% include _toc.html %}

#Antecedentes

Las organizaciones, con el pasar de los años, han cambiado, mutado y en fin, evolucionado, muchos podrían decir que la tecnología los ha forzado a esto, pero según mi parecer, las exigencias propias de las organizaciones (llamemosla empresa, sociedad, etc) son las que impulsan los cambios en la tecnología. En cualquier caso, se han vuelto mucho más complejas en cuanto a sus elementos y relaciones, además que en la actualidad las capacidades de adaptarse rápido o prever estos cambios se han vuelto necesidad. 

Por lo descrito, y muchas razones más, se han desarrollado muchas técnicas del como analizar y modelar el entorno y procesos de una o de una red de organizaciones.  Por mencionar algunas tenemos el DFD, Diagrama de Flujo, Organigramas, entre otros, los cuales en la práctica de entonces fueron suficientes para el análisis, sin embargo a medida que la complejidad fué creciendo, estas técnicas presentaban diagramas que parecían cada vez más un circuito integrado:

![](http://si2008.wikispaces.com/file/view/diagrama_de_flujo_-_incidencias.png/31827031/diagrama_de_flujo_-_incidencias.png)

Peor está [esta](http://www.cilco.co.uk/briefing-studies/acme-fashion-supplies-feasibility-study/images/top-level-dfd.jpg) que no la embebo en la entrada para no hacerla extensa innecesariamente.

Entonces, ¿como se llegó a esto?, propondré un ejercicio para entender que ni la técnica ni el ejecutor de la misma estaban equivocados, solo que excedieron el límite, aquí va el ejercicio:

 - **Paso 0**: Escoja una empresa u organización que conozca relativamente bien (procesos, áreas, interacciones).
 
 - **Paso 1**: Agarre una hoja en blanco mentalmente (o físicamente) y dibuje puntos dispersos identificándolos a cada uno con el nombre de alguna área de su empresa u organización.  Luego repita lo mismo con cada tipo de documento, proceso, roles y actores (estos últimos también conocidos como funciones y personas), sistemas, aplicaciones, servidores, computadoras, etc...  Luego de un rato debe ir quedando como lo siguiente pero con más puntos: 
 
![Puntos en Plano][puntos_plano]


 - **Paso 2**: Ahora intente trazar una línea por cada relación que vea y conozca... Seguro se le dificultará en una hoja plana, empezará a saltar encima de sus propias líneas, pero entonces, como es una hoja imaginaria, quitémonos ese problema de encima y ahora pensemos que es como un holograma, en tres dimensiones y dibujemos todas las líneas que las relacionan, seguro pensaremos en algo como esto:
 
![Madeja Ordenada][madeja_ordenada]

Pero cuando lo llevamos a la realidad es algo como esto:

![Madeja real][real_madeja]

 - **Paso 3**: Consiga el primer área que representó y dígame con cuales actores se encuentra relacionado en primer y segundo nivel... 
 
 
Tarea ardua, ¿no?. Aquí es cuando nace la necesidad de la Arquitectura Empresarial, necesitamos una herramienta que nos permita llegar, fácilmente, desde la figura A a la figura B:

[Modelo AE][modelo_ae]

#¿Que es la AE?

>AE es una práctica estratégica, que permite conectar las relaciones entre las iniciativas de negocio y la tecnología que la apalanca,  permite evaluar las fortalezas y debilidades, y trazar estrategias de transformación, desde la Arquitectura actual hacia un modelo Arquitectónico que represente una visión futura.[^1]

Es decir, la que nos permite mantener la <s>*madeja*</s> mostrada arriba unida y poderla analizar y estudiar conservando la traza de sus relaciones desde el punto más concreto como puede ser un operario y su máquina hasta los conceptos más abstractos como objetivos y metas empresariales.

#¿Para que me(nos) sirve la AE?

>La AE nos permite observar como las estrategias, metas, componentes y tecnologías están relacionadas y mostrar la interdependencia entre ellas, al final de cuentas los proyectos de tecnología deben existir exclusivamente como parte de las estrategias de negocio de la empresa.
>
>EA permite enfocar los problemas de una forma integrada y coherente, al mismo tiempo que ofrece un medio para alcanzar un entendimiento y conceptualización entre todos los involucrados en las decisiones de la empresa.[^1]

En otras palabras, conociendo todas las relaciones reales entre todos los elementos de la empresa, podremos entender mejor los problemas o iniciativas observadas y así ser más efectivos en las estrategias y tácticas de negocio a implementar para afrontar los cambios futuros y aumentar la competitividad de nuestra organización.


En próximas entregas hablaré de algunos marcos de trabajos existentes y de herramientas informáticas que nos pueden ayudar a trabajar la AE.

[madeja_ordenada]: /images/madeja_ordenada.jpg
[puntos_plano]: /images/puntos_en_plano.jpg
[real_madeja]: /images/madeja_real.jpg
[modelo_ae]: /images/triangulation.png
[^1]:http://blog.group-gqs.com/?p=72
