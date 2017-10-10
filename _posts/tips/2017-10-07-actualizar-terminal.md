---
layout: page
title:  "Actualizar desde la terminal"
subheadline:  "Tips"
teaser: "Un servicio para proveer contraseñas"
categories:
    - tips
tags:
    - terminal
    - paquetes
    - dependencias

---
En esta página te enseñamos a actualizar desde la terminal. Necesitas permisos de administrador para esos procedimientos.

Este sistema usa las "herramientas" debian package (dpkg) y aptitude (apt) para ese fín. Quizás no aplica a aplicacines independencies desarrollados bajo Flatpak/Snap.

## Pasos para actualizar
Desde la terminal, actualizamos los paquetes.
~~~
sudo apt update
~~~

En este listado verás cuandos paquetes están listos. Continúa con los comandos de mejoras (upgrade para actualizaciones menores y full-updgrade para mayores).

~~~
sudo apt upgrade && sudo apt full-upgrade
~~~

## Revisar los paquetes gráficamente
Desde la terminal, podemos echar un vistazo los paquetes instalados. A diferencia del apt original, tiene un interfaz gráfico similar a los años 90.

~~~
sudo aptitude
~~~

Debido a que no requiere la intervención del ratón, tienes que conocer los atajos de teclado (versión 0.8.6): ´q´ para retroceder o salir, ´u´ para actualizar , ´g´ para instalar o desinstalar y ´Control + T´ para ver el menú.

## Errores comunes
#### Dependencias incompletas
Si hay problemas puedes revisar en la aplicación Synaptic o realizando comandos de comprobación e instalaciones paquetes:

~~~
sudo apt-get update
sudo apt-get check
sudo apt-get -f install
~~~

#### Archivo protegido sources.list
Eso se depe a que estas interfiriendo con las actualizaciones del centro de control. Reinicia el equipo.

#### Nueva configuración disponible
Está expresada en oraciones como "El distribuidor del paquete ha publicado una version actualizada". Recomendamos aceptar los nuevos cambios (en general, escribir ´y´ y pulsar ´Enter´). Más detalles en [la sección Tips]({{ site.url }}{{ site.baseurl }}/tips/actualizar-conf-paquetes).

#### Paquetes huérfanos
Este comando sirve para eliminarlos.
~~~
sudo apt autoremove
~~~

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}aptitude.png" alt="Aplicación Aptitude.">
    </div><!-- /.medium-4.columns -->
</div>

## Lectura adicional

* [Blog de jcsis](https://jcsis.wordpress.com/2016/04/28/solucionar-el-problemas-de-dependencias-en-ubuntu-o-debian/)
* [ComputerWegne](https://computernewage.com/2015/02/22/como-instalar-aplicaciones-en-ubuntu-desde-la-terminal-con-apt-apt-get-y-aptitude/)
* [Página en Debian](https://www.debian.org/doc/manuals/aptitude/ch01s02.es.html)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
