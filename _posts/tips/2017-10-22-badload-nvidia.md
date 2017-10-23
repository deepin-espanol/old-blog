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

Si quieres saber más detalles sobre esté y más componentes en Deepin, visita [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/tips/dudas-tecnicas/).

## Pasos para retornar al driver libre Nouveau
Primero. Hacemos una copia de seguridad con [cd]({{ site.url }}{{ site.baseurl }}/tips/archivos-terminal/). `sudo mv /etc/X11/xorg.conf /etc/X11/xorg.conf.BACKUP`.:

Segundo. Tenemos dos posibilidades para retomar el driver Nouveau:
* `sudo apt install nouveau-firmware && sudo dpkg-reconfigure xserver-xorg`
* `sudo apt install xserver-xorg-video-nouveau`

Tercero. Si fuera necesario, desinstala el driver Nividia y elimina su configuración.
* `apt —purge remove nvidia-driver`
* `sudo apt remove nvidia*`

## Lectura adicional
* [Fuente AskUbuntu](https://askubuntu.com/questions/12937/remove-nvidia-driver-and-go-back-to-nouveau)
* [Freedesktop](https://nouveau.freedesktop.org/wiki/DebianInstall/)
* [Lista de controladores Nvidia](http://www.nvidia.com/object/unix.html)
* [Problemas al cargar Deepin]({{ site.url }}{{ site.baseurl }}/anexos/badload/).
* [Solución al controlador Wifi]({{ site.url }}{{ site.baseurl }}/tips/wififix/).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
