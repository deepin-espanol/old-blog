---
layout: page-fullwidth
title: "Instalación"
subheadline: "Sistema operativo"
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

Seguimos con la instalación de Deepin, específicamente la versión oficial para escritorio.

## Requisitos

Antes de usar Deepin tu equipo debe estar preparado con estos requisitos:

* 10 GB de espacio libre en el disco duro o sólido
* Procesador de **64 bits**, no importa si es Intel o AMD
* Tarjeta gráfica Intel, NVdia o AMD compatible
* 2 GB de memoria RAM, recomendamos de 4 GB a más para aprovechar al máximo

Los equipos más recientes soportan más memoria RAM ya que son de 64 bits de arquitectura. En caso que tengas problemas con la versión original, instala su versión Arch llamado [Manjaro Deepin](https://manjaro.org/category/community-editions/deepin/) que soporta 32 bis también (y es recomendado para esa arquitectura).

Para los gráficos, consulta [la página "Tarjetas de vídeo"]({{ site.url }}{{ site.baseurl }}/manual/videocard/).

## Instalación

* Arranca desde el disco o USB;
* Sigue las instrucciones;
* Selecciona la partición para el sistema y el arranque;
* La instalación demora unos minutos.

### Instalación avanzada
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>

Para establecer las particiones del disco, realiza una instalación avanzada. Eso es útil para conservar **el sistema operativo vecino** como Windows. Las particiones que debes establecer lo explicamos:

1. Añade una partición EXT4 con el arranque "/" para el sistema operativo. El mínimo es 10GB.
2. Tienes dos formas de establecer el sistema arranque, en el disco duro o en una la partición EXT4 de 300MB "/boot" (para el dual boot).
2. Otra partición "/home" para la carpeta de Mis documentos. Si establecer en un disco duro aparte de los componentes, mejor.

Revisa las páginas <a href="{{ site.url }}{{ site.baseurl }}/anexos/dudas-particiones">Dudas frecuentes</a> para mayor información.

Para complementar esta guía, sugerimos <a href="{{ site.url }}{{ site.baseurl }}/manual/dual-boot">la página Dual Boot</a> para conocer los riegos que conlleva al instalar junto a Windows. Si quieres ver otras formas de instalación recurre <a href="{{ site.url }}{{ site.baseurl }}/manual/modos-instalacion">a la página del manual</a>.

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/update/">Continúa con las actualizaciones ›</a>

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/escenciales/">Ver lista de aplicaciones escenciales ›</a>

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
