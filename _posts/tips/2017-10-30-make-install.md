---
layout: page
title:  "Usar Make Install"
subheadline:  "Tips "
teaser: "Si no es un paquete Debian o Flatpak, te enseñamos a instalar de otra forma"
breadcrumb: true
categories:
    - tips
tags:
    - fix
    - dialogo
    - apps
---
Este es un aporte para instalar ejecutables. Diferentes a los paquetes de Debian o Flatpak.

## Via archivo script
Desde el gestor de archivos puedes abrir el script con el código de abajo. Puedes comprobarlo antes de instalar el "programa".

~~~
#!/bin/sh
./configure
make
make install
~~~

Explicación: Primero establece la configuración antes, después compilas el código fuente y al último comando lo instala.

## Abriendo un archivo con cd
Si no tienes el archivo script, realízalo manualmente. Necesitas [sistema de archivos "cd" de la terminal]({{ site.url }}{{ site.baseurl }}/tips/archivos-terminal/).
1. Ejecuta con `cd`
2. `cd [lugar de codigofuente]``
3. tar –zxvf [codigofuente].tar.gz
4. cd [codigofuente]
5. ./configure
6. make
7. make install

## Fuente
* [Repositorio en Github](https://github.com/neurobin/shc)
* [Sitio web oficial](https://projects.gnome.org/gst/)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
