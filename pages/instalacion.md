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

Los equipos más recientes soportan más memoria RAM ya que son de 64 bits de arquitectura. En caso que tengas problemas con la versión original, instala su versión Arch llamado [Manjaro Deepin](https://manjaro.org/category/community-editions/deepin/) que soporta 32 bis también (y es recomendado para esa arquitectura).

Sobre las tarjetas gráficas, tal como explica el portal [Colaboratorio](https://colaboratorio.net/juan/colaboratorio/2017/tarjeta-grafica-comprar-gnulinux/), recomendamos una gráfica dedicada (o independiente) en lugar de la integrada para aprovechar los recursos a la memoria RAM. Eso puedes configurar en la Bios.

## Descarga Deepin

Hay varias maneras de descargar, además del [oficial](https://www.deepin.org/en/download/):

* [En SourceForge](https://sourceforge.net/projects/deepin/)
* [Kernel.org](http://mirrors.kernel.org/deepin-cd/)
* [Empresa en Silicon Valley, EUA](http://mirror1.sjc02.svwh.net/deepin-cd/)
* Otras formas para descargar en [la página Lista de espejos]({{ site.url }}//tips/mirror/).

Torrent:

* [En PCDS, con archivos torrent](http://www.pcds.fi/downloads/iso/debianbased/deepin/about.deepin.debian.html)
* [Linuxtracker.org, para la versión 15.4](http://linuxtracker.org/index.php?page=torrent-details&id=74fcdc5403dce919e83aa7e2c74bca2be12632a4)

Nota: Para la versión Manjaro, no oficial: [Sourcefource](https://sourceforge.net/projects/manjaro-deepin/)

Nota 2: Para descargar vía torrent es necesario un cliente compatible y comprobar la mayor cantidad de semillas, clientes encargadas de distribuir los archivos hacia otros clientes.

## Instalación en limpio

### Preparación

Cuando tengas el archivo ISO, utiliza una aplicación para copiar los archivos al USB o DVD (no CD) con Deepin Boot Maker (obviamente disponible en Deepin Store).
* Asegúrate de ser una unidad flash USB con 4 GB de almacenamiento mínimo o un DVD.
* Alternativamente puedes usar aplicaciones externas como [Rufus](https://rufus.akeo.ie/) o Unetbootin si la aplicación falla.
* Sobre Rufus, puedes usar la aplicación portátil para Windows que pesa unos megabytes.

### Instalación

* Arranca desde el disco o USB
* Sigue las instrucciones
* Para establecer las particiones del disco, realiza una instalación avanzada. No olvides de "/", "/boot", entre otros.
* La instalación demora unos minutos.

## Instalación junto a Windows

Si deseas usar Deepin junto a Windows, debes instalar de forma avanzada. Añade particiones "/", "/home" para Deepin y la carpeta de Mis documentos, recomendamos hacer en un disco duro aparte. Además, usa la partición "/boot" para establecer el doble arranque (o dual boot), si tu PC no tiene uno.

Pero al ser complicado y tedioso tener Windows y Deepin en un solo disco duro, intenta instalar Deepin con la aplicación [Deepin Windows Installer](https://www.deepin.org/it/original/deepin-installer/) para Microsoft Windows.

Advertencia: [Revisa la página Dual Boot]({{ site.url }}/manual/dual-boot/) para conocer los riegos que conlleva.

## Anexo: Vídeos explicativos
Un vídeo explicativo para instalar Deepin cortesía de Salmorejo Geek:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>
Sobre la instalación en el disco duro:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/-oswVXK8Vs0" frameborder="0" allowfullscreen></iframe>
</div>
Manjaro Deepin:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/-oswVXK8Vs0" frameborder="0" allowfullscreen></iframe>
</div>

{% include alert success='Quieres mejorar, ¡colabora con nosotros!' %}
{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
