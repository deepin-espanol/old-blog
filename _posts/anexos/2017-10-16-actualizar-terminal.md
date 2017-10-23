---
layout: page-fullwidth
title:  "Dudas al actualizar desde la terminal"
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

En esta página respondemos las dudas más comunes al actualizar Deepin desde la terminal. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/). Necesitas conocer un [poco sobre la terminal]({{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/) y tener los permisos de administrador para esos procedimientos.

{% include alert success='Esta guía forma parte de una <a href="/dudas">serie de dudas frecuentes</a> para facilitar la comprensión a todos los usuarios y usuarias' %}

***Nota:*** Este sistema usa las "herramientas" debian package (dpkg) y aptitude (apt) para ese fín. Funciona mejor con paquetes de Debian que las aplicaciones Flatpak/Snap.

***Nota 2:*** Para evitar dañar al sistema operativo, si usas el repositorio de Debian debes hacerlo manualmente. Cuando quieras actualizar Deepin desactiva ese repositorio.

## General
### ¿Cuál es el comando más sencillo para actualizar Deepin?
~~~
sudo apt update && sudo apt full-upgrade -y
~~~

Si quieres saber porqué escribir y pulsar "Enter", te explicamos en la siguiente pregunta.

### ¿Cómo actualizar paso a paso?
Si te resulta difícil, te explicamos para que sirve [sacado de las dudas sobre la terminal]({{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/): Desde la terminal, actualizamos los paquetes.
~~~
sudo apt update
~~~

En este listado verás cuandos paquetes están listos. Escribimos Upgrade es para actualizaciones. Si no funciona reemplazamos a full-updgrade para mayores.

~~~
sudo apt upgrade
~~~

Una forma más sencilla de actualizar es escribir full-upgrade y añadir `-y` al final de la sentencia. Ese últmino obliga a aceptar cualquier acción (`y` de `yes`), ahorrando tiempo (por ejemplo al aceptar cambios en la configuración, detalles en "Me avisó que hay una nueva configuración disponible").

~~~
sudo apt full-upgrade -y
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué paquetes voy a actualizar?
Para comprobar los paquetes que irás a actualizar, escribe `apt list`. No requiere derechos de administrador.

~~~
apt list —upgradable
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }


### ¿Cómo gestionar los paquetes?
Si has realizado una actualización puedes comprobar a través del Shell Aptitude. Podemos echar un vistazo los paquetes instalados. A diferencia del apt original, tiene una interfaz gráfica similar a los años 90.

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

Si los problemas persisten, revisa [la sección Dudas técnicas]({{ site.url }}{{ site.baseurl }}/anexos/dudas-tecnicas#conflicto)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Dice que el archivo está sources.list protegido
Eso se debe a que las actualizaciones centro de control están haciendo el trabajo de actualizar. Reinicia el equipo.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

#### Me avisó que hay una nueva configuración disponible
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
