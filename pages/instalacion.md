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

Para los gráficos, consulta [la página "Tarjetas de vídeo"]({{ site.url }}/manual/videocard/).

## Pasos para Deepin OS
### Descarga Deepin

Hay varias maneras de descargar, además del [oficial](https://www.deepin.org/en/download/):

* [En SourceForge](https://sourceforge.net/projects/deepin/)
* [Kernel.org](http://mirrors.kernel.org/deepin-cd/)
* [Empresa en Silicon Valley, EUA](http://mirror1.sjc02.svwh.net/deepin-cd/)
* Otras formas para descargar en [la página Lista de espejos]({{ site.url }}//tips/mirror/).

Torrent:

* [En PCDS, con archivos torrent](http://www.pcds.fi/downloads/iso/debianbased/deepin/about.deepin.debian.html)
* [Linuxtracker.org, para la versión 15.4](http://linuxtracker.org/index.php?page=torrent-details&id=74fcdc5403dce919e83aa7e2c74bca2be12632a4)

Para descargar vía torrent es necesario un cliente compatible y comprobar la mayor cantidad de semillas, clientes encargadas de distribuir los archivos hacia otros clientes.

### Preparación

Cuando tengas el archivo ISO, utiliza una aplicación para copiar los archivos al USB o DVD (no CD) con la aplicación que prefieras.

Si no conoces, te [damos una mano]({{ site.url }}/manual/discoarranque/).

### Instalación

* Arranca desde el disco o USB;
* Sigue las instrucciones;
* Selecciona la partición para el sistema y el arranque;
* La instalación demora unos minutos.

### Instalación avanzada
Para establecer las particiones del disco, realiza una instalación avanzada. Eso es útil para conservar **el sistema operativo vecino** como Windows. Las particiones que debes establecer lo explicamos:

1. Añade una partición EXT4 con el arranque "/" para el sistema operativo. El mínimo es 10GB.
2. Tienes dos formas de establecer el sistema arranque, en el disco duro o en una la partición EXT4 de 300MB "/boot" (para el dual boot).
2. Otra partición "/home" para la carpeta de Mis documentos. Si establecer en un disco duro aparte de los componentes, mejor.

Nota: Revisa [la página Dual Boot]({{ site.url }}/manual/dual-boot/) para conocer los riegos que conlleva.

## Otras formas de instalar Deepin

### Deepin Manjaro

Es una [versión no oficial](https://manjaro.github.io/Manjaro-Deepin-released/) basada en Arch en lugar de Debian. Descárgalos desde [Sourcefource](https://sourceforge.net/projects/manjaro-deepin/).

Si tienes instalado un sistema operativo, visita [la página Otras distros]({{ site.url }}/manual/otrasdistros/) para conseguir el escritorio.

### Instalación junto a Windows

Si te complica instalar Deepin con la instalación avanzada Deepin con la [aplicación para Microsoft Windows]({{ site.url }}/apps/deepininstaller/).

## Anexo: Vídeos explicativos
Un vídeo explicativo para instalar Deepin cortesía de Salmorejo Geek:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>
Sobre la instalación en el disco duro:
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/-oswVXK8Vs0" frameborder="0" allowfullscreen></iframe>
</div>

{% include alert success='Quieres mejorar, ¡colabora con nosotros!' %}
{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
