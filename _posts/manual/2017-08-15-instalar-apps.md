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

Este método no es muy recomendable como Deepin Store. Termina siendo útil para obtener versiones más actualizadas o no incluidas en la tienda.

Ten en cuenta que el sistema de paquetes usa dependencias. No funciona con aplicaciones exclusivamente diseñadas para Ubuntu, recomendamos usar vía snap en su lugar para evitar "romper" el sistema. En estos casos, la aplicación te alertará antes de instalar.

Siempre haz un respaldo de tus documentos.

1. Ejecuta Deepin Deb Installer;
2. Selecciona el paquete o arrastra varios a la vez;
3. Comprueba si hay problemas con los paquetes;
4. Si se instala correctamente, se cerrará la ventana;
5. Disfruta.

### Archivos Flatpak

Instalar vía Flatpak es una alternativa a los tradiciones deb, reduciendo las posibilidades de "dejar inoperativa al sistema operativo". Cuando es un programa Flatpak, utiliza sus propias librerías, reduciendo la dependencia con los componentes del sistema.

Es compatible con cualquier distribución Linux y te permite actualizar a la última versión de forma independiente, reduciendo la carga de trabajo a los desarrolladores.

Desde Deepin 15.5, es posible instalar. Los archivos llevan la terminación .flatpak. Para la interfaz de usuario necesitarás que el sistema operativo soporte librerías KDE, GNOME o DTK.

### Snap
Snap es otra alternativa a la instalción tradicional, desarrollada por Cannonical y está diseñada para Ubuntu. En Deepin es bastante recomendable para ejecutar aplicaciones pero tiene algunas limitaciones.

### appimage
También puedes usar los archivos "appimage", archivos comprimidos portables para ejecutar aplicaciones.  A diferencia de Flatpak y Snap, los programas sin necesidad de instalarlos.

Los archivos se guardan en una carpeta con el nombre del programa, que puedes cambiar creando una propia tipo `.miapp`.

## Otras formas
### Scripts
Hay otras formas de instalar usando scripts (archivos sh o bin). Este método es menos seguro y genera cierta inestabilidad al no usar las herramientas adecuadas. Considera crear un [acceso directo]({{ site.url }}{{ site.baseurl }}/tips/accesodirecto/) si quieres abrir desde el escritorio.

### PPA
Son las siglas de [Personal Package Archives]](https://es.wikipedia.org/wiki/Archivo_de_Paquete_Personal), ofrecidas principalmente por Lauhcpad.

## Lectura adicional
* [Dudas sobre aplicaciones]({{ site.url }}{{ site.baseurl }}/anexos/dudas-aplicaciones/)

## Lista de aplicaciones
{: .t60 }
{% include list-posts categories='apps' entries='10'%}
<!--more-->
