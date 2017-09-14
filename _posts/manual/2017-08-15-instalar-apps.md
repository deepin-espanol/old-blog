---
layout: page
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

## De forma externa (deb)

Este método no es muy seguro como Deepin Store, pero termina siendo útil para obtener versiones más actualizadas o no incluidas en la tienda.

Ten en cuenta que el sistema de paquetes usa dependencias. No funciona con aplicaciones exclusivamente diseñadas para Ubuntu, podría "romper" el sistema operativo y no arrancarlo. En estos casos, la aplicación te alertará antes de instalar.

Siempre haz un respaldo de tus documentos.

1. Ejecuta Deepin Deb Installer;
2. Selecciona el paquete o arrastra varios a la vez;
3. Comprueba si hay problemas con los paquetes;
4. Si se instala correctamente, se cerrará la ventana;
5. Disfruta.

## Con instaladores Flatpak

Instalar vía Flatpak es una forma más segura que deb. Desde Deepin 15.5, es posible instalar. Cuando es un programa Flatpak, no interfiere a los componentes del sistema, es compatible con cualquier distribución Linux y se actualizan a la última versión de forma independiente.

Los archivos llevan la terminación .flatpak. Para la interfaz de usuario necesitarás que el sistema operativo soporte librerías KDE, GNOME o DTK.

## Otras formas

Hay otras formas de instalar usando scripts (archivos sh). Este método es menos seguro y genera cierta inestabilidad.

También puedes usar los archivos "appimage", archivos comprimidos para ejecutar los programas sin necesidad de instalarlos. Aunque, algunos archivos se guardan en una carpeta con el nombre del programa.

## Lista de aplicaciones
{: .t60 }
{% include list-posts categories='apps' %}
<!--more-->