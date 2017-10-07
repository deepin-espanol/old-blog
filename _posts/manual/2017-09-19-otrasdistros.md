---
layout: page
title:  "Transplantar DDE en distros Linux"
subheadline:  "Manual"
teaser: "El escritorio de Deepin en Ubuntu y otros más"
sidebar: right
categories:
    - manual
tags:
    - distro
    - escritorio
    - dde
    - portar
    - transplantar

---
Aparte del sistema operativo Deepin, puedes portar e instalar el escritorio de entorno en distros compatibles, como Ubuntu, Linux Mint o portar por tu cuenta.

## Considera que:

Hasta la versión 14, Deepin estuvo basado en el sistema operativo Ubuntu. Sin embargo, a partir de su sucesor, Deepin usa la base, Debian Sid.

## Distribuciones transplantadas

### Distribuciones preparadas
Revisa:
* [Sabores de Deepin no oficiales]({{ site.url }}/manual/sabores/)
* [Hacer el disco de arranque]({{ site.url }}/manual/discoarranque/)

### Distribuciones que requieren instalar

Cada respositorio tiene los componentes para descargar e instalar. Desde el [sitio web oficial](https://www.deepin.org/es/dde/desktop-transplantation/) encontramos:

* Manjaro Deepin
* Arch Linux con Deepin
* [Gentoo](https://github.com/zhtengw/deepin-overlay)
* [Sparkylinux](https://sparkylinux.org/deepin-desktop-environment/)
* Ubuntu

Consulta la página de ayuda o el foro de la comunidad para ver el avance en cada distro.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/GTdVUvjTJUg" frameborder="0" allowfullscreen></iframe>
</div>

Algunas aplicaciones exclusivas requieren del entorno de escritorio, debido al kit de interfaz. Si lo usas en otros entornos, consumiría más recursos.

## Código fuente
El código fuente está en [Github](https://github.com/linuxdeepin/dde-file-manager/tree/develop2.0), que incluye el gestor de archivos, el Deepin Toolbar Kit y el centro de control.

### Requisitos

El escritorio Deepin rquiere la librería Qt 5.7, necesaria para la interfaz gráfica de las aplicaciones del sistema.

## Imagen

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}manjaro-deepin-17.0.2.png" alt="Manjaro 17.0.2">
    </div><!-- /.medium-4.columns -->
</div>

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
