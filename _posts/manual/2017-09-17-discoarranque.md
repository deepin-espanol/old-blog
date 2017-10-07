---
layout: page
title:  "Elaborar disco de arranque"
subheadline:  "Manual"
teaser: "Elabora el instalador en tu USB o DVD"
sidebar: right
categories:
    - manual
tags:
    - arranque
    - cd
    - dvd
    - usb
    - disco

---
[Instalar]({{ site.url }}/instalacion/) Deepin en una computadora de mesa o portátil requiere de una unidad de arraaque ([Boot disk](https://en.wikipedia.org/wiki/Boot_disk)).
En Deepin en Español te enseñamos a hacerlo.

## Requisitos

* Dispositivo de almacenamiento:
  - USB con 4 GB de almacenamiento mínimo
  - Un DVD. No funciona con CD.
* Cualquiera de esos programas:
  - [Rufus](https://rufus.akeo.ie/)
  - [Unetbootin](https://unetbootin.github.io/)
  - Deepin Boot Maker (disponible en Deepin Store)

Nota: En Windows, usa la aplicación portátil de Rufus que pesa unos megabytes.

## Pasos

Para Deepin Boot Maker:
1. Selecciona el archivo deepin-xx.iso (el nombre varía)
2. Escoge el dispositivo de almacenamiento
3. Confirma y espera unos minutos

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}arranque.png" alt=" Imagen de arranque">
    </div><!-- /.medium-4.columns -->
</div>

Para Rufus (solo USB):
1. Selecciona el dispositivo;
2. Haz clic en el icono al costado de "Imagen ISO" y selecciona el archivo deepin-xx.iso (el nombre varía)
3. Deja la configuración recomendada:
  - Partición GPT para computadora UEFI
  - Sistema de archivos FAT32
  - Las etiquetas "Crear disco de arranque" y "Formateo rápido" marcadas
4. Pulsa "Empezar"

Para unetbootin:
1. Selecciona "Imagen de disco" y selecciona el archivo
2. Selecciona el tipo "USB Drive" o "CD" y la unidad
3. Acepta

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}unetboot.jpg" alt="">
    </div><!-- /.medium-4.columns -->
</div>


### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
