---
layout: page
sidebar: right
sidebar: left
subheadline: Manual
title:  "Instalar aplicaciones Deepin"
teaser: "Deepin Store y más."
breadcrumb: true
tags:
    - terminal
    - apps
    - deepin
categories:
    - manual
image:
    thumb: gallery-example-3-thumb.jpg
    title: gallery-example-3.jpg
    caption_url: http://unsplash.com
---
Hay varias formas de obtener aplicaciones en *Deepin*. La forma más fácil es instalar desde la Deepin Store o externamente vía archivos DEB o Flatpak.

## Desde Deepin Store

La forma más sencilla de instalar aplicaciones es accediendo a Deepin Store. Al ingresar tendrás un buscador o selector de categorías.

Si quieres desinstalar puedes hacerlo desde el lanzador de aplicaciones.

## De forma externa
### Paquetes de Debian (deb)

Este método no es muy recomendable que el método vía Deepin Store. Termina siendo útil para obtener versiones alternativas o no incluidas en la tienda.

Ten en cuenta que el sistema de paquetes usa dependencias, para administrar usa [Synaptic]({{ site.url }}{{ site.baseurl }}/apps/synaptic/). No funciona con aplicaciones exclusivamente diseñadas para Ubuntu, recomendamos usar otros métodos en su lugar.

Para instalar un paquete de Debian suelto o varios de ellos:

1. Ejecuta Deepin Deb Installer;
2. Selecciona el paquete o arrastra varios a la vez;
3. Comprueba si hay problemas con los paquetes;
4. Si se instala correctamente, se cerrará la ventana;
5. Ejecuta desde el lanzador de aplicaciones.

### Archivos Flatpak

Instalar vía Flatpak es una alternativa a los tradiciones deb, reduciendo las posibilidades de "dejar inoperativa al sistema operativo". Cuando es un programa Flatpak, utiliza sus propias librerías, reduciendo la dependencia con los componentes del sistema.

Es compatible con cualquier distribución Linux y te permite actualizar a la última versión de forma independiente, reduciendo la carga de trabajo a los desarrolladores. La documentación lo encontrarás en la [sección Técnico]({{ site.url }}{{ site.baseurl }}/tecnico/flatpak/).

Desde Deepin 15.5, ya es posible instalar aplicaciones de ese tipo. Los "instaladores" llevan la terminación .flatpak. Para instalar es necesario un entorno de arranque KDE, GNOME o DTK, dependiendo de la librería gráfica, incluida en el sistema operativo.

### Snap
Snap es otra alternativa a la instalción tradicional, desarrollada por Cannonical y está diseñada para Ubuntu. En Deepin es bastante recomendable para ejecutar aplicaciones pero tiene algunas limitaciones.

### appimage
También puedes usar los archivos "appimage", archivos comprimidos portables para ejecutar aplicaciones.  A diferencia de Flatpak y Snap, los programas sin necesidad de instalarlos.

Los archivos se guardan en una carpeta con el nombre del programa, que puedes cambiar creando una propia tipo `.miapp`.

## Otras formas
### Ejecutables sueltos
La instalaciones vía script (extensiones `sh` o `run`) o binarios (extensión `bin`) son diferentes a los paquetes de Debian o Flatpak. Para este método necesitarás conocer el código fuente y su estado de desarrollo. El código fuente está dentro de ejecutable o comprimido en tarball (extensiones tar.gz o tgz).

Para instalar, realiza en [Make Install]({{ site.url }}{{ site.baseurl }}/tips/make-install/). En ocasiones se traslada la información sin acceso directo; si eso sucede, considera [crearlo uno]({{ site.url }}{{ site.baseurl }}/tips/accesodirecto/).

Recuerda, si notas que el [código fuente está ofuscado]({{ site.url }}{{ site.baseurl }}/tips/ofuscar-scriptbash/) y proviene de un sitio web desconocido, ***no lo ejecutes***.

### PPA
Son las siglas de [Personal Package Archives]](https://es.wikipedia.org/wiki/Archivo_de_Paquete_Personal), ofrecidas principalmente por Lauhcpad. Esta opción [es útil para los desarrolles]({{ site.url }}{{ site.baseurl }}/actividades/hacerppa).

## Lectura adicional
* [Dudas sobre aplicaciones]({{ site.url }}{{ site.baseurl }}/anexos/dudas-aplicaciones/)
* [Artículo en Linuxadictos](https://www.linuxadictos.com/tutorial-como-instalar-cualquier-paquete-en-gnulinux.html)

## Lista de aplicaciones
{: .t60 }
{% include list-posts categories='apps' entries='10'%}
<!--more-->
