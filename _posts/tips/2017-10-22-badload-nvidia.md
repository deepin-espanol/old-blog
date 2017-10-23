---
layout: page
title:  "Solución al problema de no cargar en tarjetas Nvidia"
subheadline:  "Tips "
teaser: "Cómo arreglar la tarjeta Nvidia mal instalada"
categories:
    - tips
tags:
    - driver
    - nvidia
    - boot
---
Uno de los problemas al arrancar el equipo es iniciar con una pantalla vacía y pocos textos, es decir [en modo TTY]({{ site.url }}{{ site.baseurl }}/tips/tty/). Eso se debe a que no cargó el controlador.

Si quieres saber más detalles sobre esté y más componentes en Deepin , visita [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/tips/dudas-tecnicas/).

## Pasos
1. Desinstala `apt —purge remove nvidia-driver`
<!--TODO: Mejorar-->


## Lectura adicional
* [Lista de controladores Nvidia](http://www.nvidia.com/object/unix.html)
* [Problemas al cargar Deepin]({{ site.url }}{{ site.baseurl }}/anexos/badload/).
* [Solución al controlador Wifi]({{ site.url }}{{ site.baseurl }}/tips/wififix/).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
