---
layout: page
title:  "Dudas al actualizar desde la terminal"
subheadline:  "Anexo"
teaser: "Un servicio para proveer contraseñas"
categories:
    - anexos
tags:
    - terminal
    - dudas
    - paquetes
    - dependencias

---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Índice**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
{% include _improve_content.html %}

En esta página respondemos las dudas más comunes al actualizar Deepin desde la terminal. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/). Necesitas conocer un [poco sobre la terminal]]({{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/) y tener los permisos de administrador para esos procedimientos.

***Nota:*** Este sistema usa las "herramientas" debian package (dpkg) y aptitude (apt) para ese fín. Funciona mejor con paquetes de Debian que las aplicaciones Flatpak/Snap.

## General
### ¿Cómo actualizar desde la terminal?
Desde la terminal, actualizamos los paquetes.
~~~
sudo apt update
~~~

En este listado verás cuandos paquetes están listos. Continúa con los comandos de mejoras (upgrade para actualizaciones menores y full-updgrade para mayores).

~~~
sudo apt upgrade && sudo apt full-upgrade
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo revisar los paquetes?
Desde la terminal, podemos echar un vistazo los paquetes instalados. A diferencia del apt original, tiene un interfaz gráfico similar a los años 90.

~~~
sudo aptitude
~~~

Debido a que no requiere la intervención del ratón, tienes que conocer los atajos de teclado (versión 0.8.6): ´q´ para retroceder o salir, ´u´ para actualizar , ´g´ para instalar o desinstalar y ´Control + T´ para ver el menú.

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}aptitude.png" alt="Aplicación Aptitude.">
    </div><!-- /.medium-4.columns -->
</div>

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Errores comunes
#### Veo el mensaje "Dependencias incompletas"
Si hay problemas puedes revisar en la aplicación Synaptic o realizando comandos de comprobación e instalaciones paquetes:

~~~
sudo apt-get update
sudo apt-get check
sudo apt-get -f install
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Dice que el archivo está sources.list protegido
Eso se debe a que las actualizaciones centro de control están haciendo el trabajo de actualizar. Reinicia el equipo.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Me aviso que hay una nueva configuración disponible
Está expresada en oraciones como "El distribuidor del paquete ha publicado una version actualizada". Recomendamos aceptar los nuevos cambios (en general, escribir ´y´ y pulsar ´Enter´). Más detalles en [la sección Tips]({{ site.url }}{{ site.baseurl }}/tips/actualizar-conf-paquetes).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Hay paquetes huérfanos
Este comando sirve para eliminarlos.
~~~
sudo apt autoremove
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### No puedo instalar porque los paquetes están corruptos
Este comando sirve para limpiar la caché.
~~~
sudo apt-get clean
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Lectura adicional

* [Blog de jcsis](https://jcsis.wordpress.com/2016/04/28/solucionar-el-problemas-de-dependencias-en-ubuntu-o-debian/)
* [ComputerWegne](https://computernewage.com/2015/02/22/como-instalar-aplicaciones-en-ubuntu-desde-la-terminal-con-apt-apt-get-y-aptitude/)
* [Página en Debian](https://www.debian.org/doc/manuals/aptitude/ch01s02.es.html)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
