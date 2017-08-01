---
layout: page-fullwidth
title: "Instalación"
subheadline: "En unos minutos"
teaser: "Esta página explica como instalar"
permalink: "/instalacion/"
header:
   image_fullwidth: "wallpaper.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
{% include _improve_content.html %}

## Requisitos

Antes de usar Deepin tu equipo debe estar preparado con estos requisitos:

* 10 GB de espacio libre en el disco duro o sólido
* Procesador de **64 bits**, no importa si es Intel o AMD
* Tarjeta gráfica Intel, NVdia o AMD compatible
* 2 GB de memoria RAM, recomendamos de 4 GB a más para aprovechar al máximo

Sobre las tarjetas gárficas, tal como explica el portal [Colaboratorio](https://colaboratorio.net/juan/colaboratorio/2017/tarjeta-grafica-comprar-gnulinux/), recomendamos una gráfica dedicada en lugar de la integrada para aprovechar la memoria RAM. Eso puedes configurar el la Bios.

## Descarga Deepin

Hay varias maneras de descargar, además del [oficial](https://www.deepin.org/en/download/):

* [En SourceForge](https://sourceforge.net/projects/deepin/)
* [En PCDS, con archivos torrent](http://www.pcds.fi/downloads/iso/debianbased/deepin/about.deepin.debian.html)

## Instalación en limpio

### Prepara el instalador

Cuando tengas el archivo ISO, utiliza una aplicación para copiar los archivos al USB o DVD (no CD) con Deepin Boot Maker.
* Asegúrate de ser una unidad flash USB con 4 GB de almacenamiento mínimo o un DVD.
* Alternativamente puedes usar aplicaciones externas como [Rufus](https://rufus.akeo.ie/) o Unetbootin si la aplicación falla.


### Video instalación

Un vídeo explicativo para instalar Deepin tanto el modo básico como el avanzado cortesía de Salmorejo Geek:

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>

## Instalación junto a Windows

Si deseas usar Deepin junto a Windows, puedes aplicar una partición especial y establecer las particiones /home y /boot para establecer el doble arranque (o dual boot).

Pero al ser complicado y tedioso, intenta instalar Deepin con la aplicación [Deepin Windows Installer](https://www.deepin.org/it/original/deepin-installer/) para Microsoft Windows.

{% include alert success='Quieres mejorar, ¡colabora con nosotros!' %}
{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
