---
layout: page
title:  "Deepin Clone"
subheadline:  "Manual"
teaser: "Respaldo de archivos en Deepin"
sidebar: right
breadcrumb: true
categories:
    - manual
tags:
    - clone
    - backup
    - particiones
    - originales
image:
    title: header_unsplash_7
---

Deepin Clone es una aplicación para respaldar contenido del disco duro.

## Interfaz
Funciona con particiones y discos duros completos. Se tranfiera en una nueva partición o una imagen de disco.

Puedes guardar las imagenes en discos duros externos sean NTFS o EXT4. Sin embargo, no es compatible con formato FAT porque almacenan archivos hasta 4 GB.

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}deepinclone.png" alt="Sección de inicio de Deepin Clone">
    </div><!-- /.medium-4.columns -->
</div>

## Nota
Para hacer o restaurar copias de seguridad de particiones del sistema es necesario instalar Deepin Recovery. Viene incluido en Deepin 15.5. En la terminal se instala con `sudo apt-get install live-filesystem`.

Deepin Recovery se accede en el menú de arranque.

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}deepinrecovery3.png" alt="Deepin Clone en Deepin Recovery">
    </div><!-- /.medium-4.columns -->
</div>

## Lectura adicional
* [Deepin Recovery]({{ site.url }}{{ site.baseurl }}/manual/deepin-recovery)

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
