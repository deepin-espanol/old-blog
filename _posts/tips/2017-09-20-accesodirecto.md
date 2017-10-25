---
layout: page
#
# Content
#
subheadline: "Tip"
title: "Accesos directos personalizados"
teaser: "Cómo crear o modificar un acceso directo para tu aplicación"
breadcrumb: true   
categories:
  - tips
tags:
  - aplicacion
  - enlace
  - acceso
  - modificar

---

En casos que no consigues [acceder a la aplicación]({{ site.url }}{{ site.baseurl }}/manual/instalar-apps/), sea por ser su naturaleza de portable o que la instalación está incompleta, te recomendamos crear un acceso directo.

## Cómo crearlo

1. Ir a la carpeta ´usr/share/applications/´
2. Crea el archivo ´nombreprograma.desktop´
3. Edítala (la explicación debajo)

## Qué contiene el archivo

El archivo ´nombreprograma.desktop´ contiene este código:

~~~
[Desktop Entry]
Name=Nombre del programa
Comment=Descriptción sobre el programa
Exec=/home/usuario/carpetaPrograma/bin/programa.sh
Icon=/home/usuario/Images/iconoPrograma
Terminal=false
Type=Application
~~~

Name es el nombre del programa, Comment la descripción e Icon el logotipo de la aplicación (preferible PNG). El ejecutable debe indicar la ruta de la aplicación (los ejecutables son archivos .sh, análogos al .exe).

## Lectura adicional
* [Linuxadictos](https://www.linuxadictos.com/crear-accesos-directos-ubuntu.html)
* [GeekTheory](https://geekytheory.com/como-crear-un-lanzador-o-acceso-directo-en-ubuntu)
