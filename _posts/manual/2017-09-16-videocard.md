---
layout: page
title:  "Tarjeta de vídeo"
subheadline:  "Manual"
teaser: "Revisando la calidad gráfica"
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

* AMD: El recomendado es AMDGPU para la marca. Otra versión y siendo comercial es AMDGPUPRO.
* Intel: Tiene un controlador propio
* Nvidia: El libre es Nouveau y el propietario es Nvidia. Algunos controladores para laptops llevan el nombre de Bumbelee.

## Vídeo
AMD:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/sHoC9nZNcS0" frameborder="0" allowfullscreen></iframe>
</div>

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
