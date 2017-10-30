---
layout: page
title:  "Ofuscar código script en terminal con Bash"
subheadline:  "Tips "
teaser: "Un truco para hacer el ejecutable con código inaccesible"
breadcrumb: true
categories:
    - tips
tags:
    - fix
    - dialogo
    - apps
---
Este es un aporte para conocer cómo ofuscar el código de un script. Debes tener en cuenta que un ejecutable de ese tipo es innaccesible y podría ocultar malware. El simple hecho de ofuscar código, deja de ser software libre y debes sospechar de ello.

Ese método también es usado para generar comandos para acceder servicios, ocultando la contraseña. Sin embargo, no recomendamos ese método usando liberías de hash en su lugar.

## Pasos con Shell script compiler
1. Descarga el comprimido que lleva Shell script compiler o `shc`
2. Extraemos y localizamos la carpeta con `cd`
3. Ejecuta con `ln -s shc-3.8.9.c shc.c`, shc-3.8.9 es la versión del ejecutable
4. Instalado con `sudo make install` (requiere tener los paquetes `gcc` y `make`)
5. Localizamos la dirección del script en cuestión
6. Ejecutamos con `shc -v -f $HOME/script.sh` (`$HOME` es la carpeta de usuario)
7. Nos genera los scripts `script.sh.x` (el que usaremos) y `script.sh.x.c` (el que no)
8. Ya está lista

## Fuente
* [Repositorio en Github](https://github.com/neurobin/shc)
* [Sitio web oficial](https://projects.gnome.org/gst/)
* [Documentación](https://linux.die.net/man/1/shc)

## Lectura adicional
* [Ver los archivos desde la terminal]({{ site.url }}{{ site.baseurl }}/tips/archivos-terminal/).
* [Usando Make Install]({{ site.url }}{{ site.baseurl }}/tips/make-install/)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
