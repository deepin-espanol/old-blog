---
layout: page-fullwidth
title: "Dudas sobre la terminal en Deepin"
teaser: "Si te complicas con las órdenes, escríbelas"
categories:
    - anexos
tags:
    - dudas
    - comunidad
header:
   image_fullwidth: "hot.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Índice**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
{% include _improve_content.html %}

En la *Comunidad Deepin* aclaramos que el sistema operativo  perfecto no existe. Buscamos que cualquiera conozca Deepin, como si fuera un vehículo o una ciudad.

En esta página respondemos las dudas relacionadas al uso de la terminal. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/). .

{% include alert success='Esta guía forma parte de una <a href="/dudas">serie de dudas frecuentes</a> para facilitar la comprensión a todos los usuarios y usuarias' %}

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Listado
### ¿Qué es la terminal?
El terminal es un componente básico que funciona al iniciar el sistema operativo. Desde los primeros años es parte importante para realizar tareas. Debido a las limitaciones de la época, este entorno tiene una intefaz basada en letras, símbolos y espacios.

Una de las computadoras que aprovechó este componente fue el [Commondare 64](https://es.wikipedia.org/wiki/Commodore_64). Sin embargo, con la ya avanzada interfaz gráfica (GUI) de los años 2000, la terminal quedó en segundo plano para el usuario común.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué es un shell?
Es el intérprete de comandos, una especie de programa que se ejecuta con órdenes. No confundir con las aplicaciones gráficas.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿La terminal te hace inteligente?
No. Algunas películas o producciones de ficción estereotiparon el uso de la terminal. Por ejemplo, [Jonny Lee Miller y Angelina Jolie en Hackers](https://en.wikipedia.org/wiki/Hackers_(film)).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Los comandos de la terminal son las mismas con las de Windows?
No. Si has usado "Símbolo de sistema" en Windows, las órdenes tienen algunas diferencias. SI piensas dar una orden a una shell tendrás que escribir `help` para conocer el listado de órdenes de un shell.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué es sudo?
Es una palabra para que el shell realice activiades del sistema. Se debe anteponer `sudo` antes de la frase:

{% include alert terminal='sudo apt update' %}

Algunas shells no pueden ejecutarse sin el sudo antepuesto. Sin embargo, debes tener cuidado al usarlas.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Ejemplos
Estos son algunos comandos que puedes descubrir. En estos casos, no necesitas escribir "sudo", o sea pedir permisos de administrador.


### Actualizar el equipo
Del anexo [Actualizar con la terminal]({{ site.url }}{{ site.baseurl }}/anexos/actualizar-terminal/).

{% include alert terminal='apt update' %}

### Mostrar detalles del sistema
Para mostrar los detalles del equipo sin recurrir a otros programas necesitarás el shell ´inxi´ para ejecutar este comando:

{% include alert terminal='inxi -Fx' %}

### Mostrar detalles del sistema
Del shell `debian-goodies` podrás saber las 15 aplicaciones que más quitan espacio en el disco. Aquí usamos dos comandos, mostados con guión:

{% include alert terminal='dpigs -n15 -H' %}

## Seguimos creciendo

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
