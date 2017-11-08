---
layout: page
title:  "Controladores"
subheadline:  "Manual"
teaser: "Qué y cómo funciona el controlador"
sidebar: right
breadcrumb: true
categories:
    - manual
tags:
    - driver
    - dispositivos
---

Deepin usa controladores, una palabra que indica el "control" a un dispositivo.

## Sobre el controlador
Un controlador (también "driver" o "rutina") es un software encargado de enviar y recibir información del dispositivo y es el intermediario del sistema operativo.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/d5BQwOowSiA" frameborder="0" allowfullscreen></iframe>
</div>

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Para qué sirve el controlador
El controlador, mayormente un DKMS, cubre a
* Tarjetas gráficas
* Placa madre o Motherboard
* Lectora de disco
* Impresoras
* Micrófonos
* Altavoces o parlantes
* Y muchos más...

Hay varios métodos, por ingeniería inversa (el controlador fue elaborado por un conocedor del tema), la comunidad de Linux o el proveedor (oficialmente).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Controladores y los gráficos
Algunos controladores gráficos usan [OpenGL](https://www.opengl.org/) y Vulkan (bajo el auspicio del Grupo Khronos) para ejecutar aplicaciones con imágenes sofisticadas. Incluso los juegos de Windows compatibles con OpenGL tienen [la posibilidad de funcionar en Deepin]({{ site.url }}/manual/exeapps/) como alternativa a Direct3D.

Para ejecutar un videojuego dependerás de la versión de OpenGL que está diseñada. La versión 1, anunciada en 1992, incluyó algunas funciones que fueron descartadas en la versión 3 de 2008. En OpenGL 4, se integra Vulkan para mejorar de rendimiento en gráficos 3D y funciona en otros sistema operativos (siempre y cuando la tarjeta de vídeo sea compatible con esa versión).

En resumen, cuando más reciente es el modelo de la tarjeta gráfica, más posibilidades de tener gráficos y detallados y fluídos con el controlador.

## ¿Cómo consigo el controlador?
En GNU/Linux, cada paquete que hacer funcionar dispositivo se le conoce como "DKMS" (Dynamic Kernel Module Support). El núcleo de Linux incluye gran parte de ellos, la comunidad se encarga de mejorar y, en el mejor de los casos, [puedes editar el código fuente al antojo]({{ site.url }}/anexos/dudas-softlibre/).

En cambio, si no tienes uno de ellos, necesitarás conseguir por separado sea en la página web (buscando por DKMS) o por [respositorios]({{ site.url }}/manual/espejos/). Es posible que algunas distribuciones no incluyan los binarios por motivos de licencia.

Revisa las [Dudas sobre los controladores]({{ site.url }}{{ site.baseurl }}/tips/dudas-drivers/), te guiaremos en los problemas de los dispositivos.

## Lectura adicional
* [Blog de usuario Debian](https://usuariodebian.blogspot.com/2011/04/dkms-dynamic-kernel-module-support.html)
* [Dudas sobre los controladores]({{ site.url }}{{ site.baseurl }}/tips/dudas-drivers/)

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
