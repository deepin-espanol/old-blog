---
layout: page
title:  "Tarjeta de vídeo"
subheadline:  "Manual"
teaser: "Revisando la calidad gráfica"
sidebar: right
categories:
    - manual
tags:
    - graficos
    - juegos
    - tarjeta

---

Antes de [jugar]({{ site.url }}/apps/juegos/), incluyendo [PlayonLinux]({{ site.url }}/apps/playonlinux/), necesitarás una tarjeta gráfica.

## Por qué una tarjeta gráfica

Las [tarjetas gráficas](https://es.wikipedia.org/wiki/Tarjeta_gr%C3%A1fica) son placas que conectan con las computadoras para ofrecer gráficos. Las tarjetas se conectan con los monitores o televisores

Tenemos dos tipos: la integrada que tiene limitaciones con el 3D y viene por defecto; y la dedicada que muestra gŕaficos en una placa independiente, con mayor potencia y tiene un coste mayor.

Tal como explica el portal [Colaboratorio](https://colaboratorio.net/juan/colaboratorio/2017/tarjeta-grafica-comprar-gnulinux/), puedes configurar en la Bios. Si usas la tarjeta dedicada, los gráficos no interferirán al consumo de RAM.

## Controladores
Algunos controladores son mantenidos por [desarrolladores]({{ site.url }}{{ site.baseurl }}/actividades/drivers/) y otros son elaborados por empresas.

* AMD: El recomendado es AMDGPU para la marca.
* Intel: Tiene un controlador propio.
* Nvidia: El libre es Nouveau y el propietario es Nvidia. Algunos controladores para laptops llevan el nombre de Bumbelee.

Algunos proveedores de drivers ofrecen un enlace para obtener los instaladores exclusivos:
* AMD con su versión comercial AMDGPUPRO.
* [Intel Graphics](https://www.linuxquestions.org/questions/linux-deepin-101/intel-linux-graphics-installer-4175539264/)
* [NVidia]({{ site.url }}/apps/install-ejecutable-nvidia/).

## OpenGL y Vulcan
Algunos controladores integran el funcionamiento gráfico para ejecutar videojuegos con la mayor calidad posible. Esas tecnologías más estandarizadas y abiertas son [OpenGL](https://www.opengl.org/) y Vulkan. Para que puedas disfrutar de los juegos, comprueba si es compatible con esas tecnologías, incluso los juegos de Windows compatibles con OpenGL tienen [la posibilidad de funcionar en Deepin]({{ site.url }}/manual/exeapps/).

Si tienes algunos problemas con los juegos, tendrás que revisar la versión soportada de OpenGL. En cambio, si tu equipo es de 2016 y posteriores puedes usar su tecnología sucesora, Vulkan, para tener la mejor calidad posible.

## Vídeo
AMD:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/sHoC9nZNcS0" frameborder="0" allowfullscreen></iframe>
</div>

## Lectura adicional
* [Dudas sobre controladores]({{ site.url }}/anexos/dudas-drivers/)

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
