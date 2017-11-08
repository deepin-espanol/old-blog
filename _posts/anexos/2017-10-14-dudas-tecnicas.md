---
layout: page-fullwidth
title: "Dudas técnicas sobre Deepin"
teaser: "Para que los especialistas conozcan a detalle"
categories:
    - anexos
tags:
    - dudas
    - comunidad
header:
   image_fullwidth: "hot.jpg"
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

En la *Comunidad Deepin* aclaramos que el sistema operativo  perfecto no existe. Buscamos que cualquiera conozca Deepin, como si fuera un vehículo o una ciudad.

En esta página respondemos las dudas más profundas. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/). Está dedicada a personas que buscan conocer el mecanismo de dicho software.

{% include alert success='Esta guía forma parte de una <a href="/dudas">serie de dudas frecuentes</a> para facilitar la comprensión a todos los usuarios y usuarias' %}

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Preámbulo y motivaciones
Queremos explicarte cómo funciona Deepin con las tres primeras preguntas indispensables y una cuarta explicando el motivo.
### ¿Qué es GNU? ¿En qué lenguaje está escrito?
GNU es el primer paso y el pilar para el desarrollo del sistema operativo. Desarrollado Richard M. Stallman en 1983 busca adoptar tecnologías informáticas (hasta entonces dominaba Unix) y hacerlo accesible para los desarrolladores sin restricciones.

Sin embargo, debido a que GNU necesitaba un núcleo para que comunique entre el software libre. En 1991 nació Linux por Linus Torvalds y un año después se formó GNU/Linux.

Como dato adicional, GNU usa un [intérprete de código fuente a binario](https://www.gnu.org/software/libc/libc.html), por lo que está escrita en C inicialmente.

Fuente: [FSF](https://www.gnu.org/gnu/gnu-linux-faq.es.html#why)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué es Linux?
Es el núcleo del sistema operativo y el más usado. Es el propio Linus Torvalds quien desarrolló y contiene información elemental como controladores de vídeo, de disco duro y muchas más.

Hasta octubre de 2017, entre las versiones 4.8 y 4.13, el primero LTS, hubo 83 000 cambios admitidos de 4300 desarrolladores de 519 corporaciones. Esa 4.13 tiene más de 24.7 millones líneas de código escritas en más de 60 000 archivos.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/UUJ0dFpj1-M" frameborder="0" allowfullscreen></iframe>
</div>
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/o8NPllzkFhE" frameborder="0" allowfullscreen></iframe>
</div>

Fuente: [Fossbytes](https://fossbytes.com/linux-kernel-development-contributer/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué es Debian?
[Debian GNU/Linux](https://es.wikipedia.org/wiki/Debian_GNU/Linux) es uno de los proyectos más vetaranos desde 1993. Es la que llamaremos "distribución", porque se encarga de distribuir, organizar y ejecutar una serie de herramientas de software, llamados "paquetes".

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/IS9WE6V-1lc" frameborder="0" allowfullscreen></iframe>
</div>

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Por qué Deepin depende parcialmente de Debian?
Para que no te compliques demasiado, Deepin es la distribución hija de Debian. Y Debian es una de las distribuciones más vetaranas.

Hasta las versión 2014 estuvo basado en Ubuntu, también basada en Debian y una de las más conocidas en los años 2000. En la versión 15.x se cambió a Debian para ganar estabilidad (
[Muy Linux](http://www.muylinux.com/2015/12/31/deepin-15/)).

Si tienes dificultades con la base Debian, puedes usar a sus tios. La versión Manjaro Deepin está basada en Arch y emplea otras tecnologías a profundidad. [Revisa la página Instalación]({{ site.url }}{{ site.baseurl }}/instalacion/). Recuerda que no está siendo desarrollado oficialmente, sino por la comunidad.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Deepin a fondo
### ¿Cómo administra los recursos y componentes del sistema Deepin? {#paquetes}
Deepin usa paquetes de Debian (extensiones "deb"). La mayoría de paquetes contienen código que se ramifica con paquetes más simples (es como un árbol de paquetes). Por ejemplo, el paquete principal es linux, y sus consecuentes están relacionados a los gráficos (Mesa), la libería gráfica (Qt), códecs, entre otros.

Deepin consigue los paquetes de la rama no estable de Debian (sid). Sin embargo, actualizar paquetes a una versión más reciente genera el "conflicto de dependencias", sobretodo en aplicaciones recientes o correcciones. Para evitar esos malestares, gran parte de las tecnologías dependen de Flatpak (desde 15.5) y las no diseñadas para Flatpak seguirán con el modelo tradicional (por ejemplo, la parte crítica de Debian).

### ¿Deepin vela por tu seguridad? ¿Cómo podemos saberlo?
Los desarrolladores publican parches [en su blog](https://www.deepin.org/en/security-update/). Además, el proyecto Debian [tiene una página web](https://www.debian.org/security/) para estar al tanto con los paquetes antes de ser distribuidos. En el caso Linux, el núcleo del sistema [está siendo auditado frecuentemente](https://lamiradadelreplicante.com/2017/09/01/agencia-alemana-de-ciberseguridad-el-generador-de-numeros-aleatorios-de-linux-es-seguro/).

En resumen, los componentes recibirán **actualizaciones críticas**.

Aún así, si tienes experiencie en cíberseguridad, [revisa el código fuente y reporta cualquier anomalía]({{ site.url }}{{ site.baseurl }}/actividades/audiar-deepin/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo funciona el entorno gráfico? ¿Qué componentes?
Deepin tiene su entorno gráfico llamado [Deepin Evolment Desktop]({{ site.url }}{{ site.baseurl }}/tecnico/api/). Es bastante simple que tienes a [Deepin Store]({{ site.url }}{{ site.baseurl }}/manual/instalar-apps/) para instalar aplicaciones a unos clics.

Otras tecnologías están relacionadas a la libería Qt, al entorno de escritorio (cuyo prefijo es dde) o los gráficos al monitor (X.org). Recuerda que son componentes muy importantes. Si te avisa que se desinstalará esos paquetes, ¡no lo hagas! Eso sucedió una cantidad pequeñísima de veces.

Fuente: [Manual de Debian](https://www.debian.org/doc/manuals/aptitude/ch02s03s02.es.html)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Deepin usa el núcleo de Linux?
Sí. El núcleo está basado en una versión a largo plazo (LTS) y modificado por los desarrolladores. Revisa el [código fuente]({{ site.url }}{{ site.baseurl }}/source) y las actividades que [puedes colaborar]({{ site.url }}{{ site.baseurl }}/actividades/kernel/).

Si tienes problemas con el núcleo, visita [la página para cambiar el núcleo de Linux]({{ site.url }}{{ site.baseurl }}/tips/kernel/).
<img class="t60" src="{{ site.urlimg }}Esquema de un sistema GNU_Linux" alt="Esquema de Linux">

Fuente: [Slideplayer](http://slideplayer.es/slide/106215/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué servicios del sistema (alias, "demonios" o "residentes") usa Deepin?
Un "demonio" es una traducción de "Daemon" y, a la vez, las siglas de Disk And Execution MONitor. Los demonios también tienen paquetes de Debian para actualizarse.

Deepin tiene un programa llamado [systemd](https://en.wikipedia.org/wiki/Systemd) (demonio del sistema). Este componente, que es un conjunto de servicios, permite comprobar los dispositivos activados durante su encendido. Así, indica que está funcionando y avisa si encuentra algún error. Puedes configurarlo [con chkservice]({{ site.url }}/tips/cambiar-servicios-systemd/).

<img class="t60" src="{{ site.urlimg }}header_homepage_13.jpg" alt="Paisaje">

Para crear servicios de systemd consulta [este artículo](https://www.redeszone.net/2017/09/02/crear-servicios-daemon-ubuntu-systemd/). Para otros demonios menores de la distro madre, visita [Demonios de Debian](https://wiki.debian.org/es/Daemon#Demonios_de_Debian).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Aplicaciones
### ¿Cómo gestiona las aplicaciones? ¿Qué recomendamos?
Viendo tu mismo. La forma más sencilla es desde el [lanzador]({{ site.url }}{{ site.baseurl }}/manual/launcher/). Los más experimentados lo hacen desde [Synaptic]({{ site.url }}{{ site.baseurl }}/apps/synaptic/)

Empaquetar a Flatpak permite a los desarrolladores tener las últimas mejoras de sus aplicaciones sin problemas. Sus componentes se actualizan de forma silenciosa y no interfieren con los componentes del sistema. Flatpak es desarrollado por la comunidad.

Por su puesto, las [aplicaciones originales]({{ site.url }}{{ site.baseurl }}/originales/) están integradas bajo Flatpak por defecto. Disponibles desde la versión 15.5 del sistema operativo. Si quieres conocer este método de instalación visita [flatpak.org](http://flatpak.org/apps.html) o nuestra [página técnica]({{ site.url }}{{ site.baseurl }}/tecnico/flatpak/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo ejecutar aplicaciones que no sean Flatpak?
Sí. Por ejemplo a Snap, por Cannonical, enfocada en Ubuntu. Está opción es compatible con Deepin para evitar el problema de Dependencias. Otras formas lo puedes consultar en [nuestro manual]({{ site.url }}{{ site.baseurl }}/manual/instalar-apps/).

### ¿Puedo ejecutar aplicaciones pesadas?
Si usas aplicaciones pesadas exclusivas de Microsoft Windows a Deepin, visita [Dudas sobre aplicaciones]({{ site.url }}{{ site.baseurl }}/anexos/dudas-aplicaciones/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo conseguir una aplicación para que funcione el dispositivo?
Sí. Echa un vistazo [al anexo]({{ site.url }}{{ site.baseurl }}/anexos/dudas-drivers/). Por defecto el núcleo Linux posee controladores para que funcionen los dispositivos (impresoras, tarjetas de vídeo, etcétera).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Miscelánea
### ¿Qué son los permisos de superusuario o administrador (root)?
Son permisos que permiten modificar los componentes del sistema. Ese permiso no se activa por defecto y necesitarás confirmar primero. Más detalles en el [manual]({{ site.url }}{{ site.baseurl }}/manual/usuarios-root/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Deepin tiene modo live?
Sí. Este modo te resultará útil para reparar la partición o probar el sistema antes de instalar. En la versión 15.4 está disponible en la opción "failsafe".

Fuente: [Gamblisfx](https://web.archive.org/web/20170606022618/http://gamblisfx.com/how-to-create-deepin-15-4-live-usb-from-linux/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Es posible filtrar contenido de la web?
Sí. Como [el cortafuegos]({{ site.url }}{{ site.baseurl }}/apps/gufw/) o [la edición del archivo de configuración "host"]({{ site.url }}{{ site.baseurl }}/tips/editar-host/).

Fuente: [Gamblisfx](https://web.archive.org/web/20170606022618/http://gamblisfx.com/how-to-create-deepin-15-4-live-usb-from-linux/)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo cifrar la carpeta Mis documentos?
Sí. Echa un vistazo [al tip]({{ site.url }}{{ site.baseurl }}/tips/cifrar-docs/). Por el momento, en Deepin 15.4 no tienes la opción de cifrar desde el centro de control.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo ahorrar y diagnosticar el consumo de energía?
Sí. Echa un vistazo [al tip]({{ site.url }}{{ site.baseurl }}/tips/ahorro-energia/). El centro de control tiene algunas opciones, por curiosidad.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Qué contenido adicional sobre Linux me recomiendas?
Si quieres estar más al tanto sobre Deepin, [al directorio extra]({{ site.url }}{{ site.baseurl }}/anexos/directorio-extra/). Hay personas como tú que también están usando GNU/Linux de forma normal.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Seguimos creciendo
Si aún no encuentras tu pregunta, usa el [Buscador]({{ site.url }}{{ site.baseurl }}/search/).

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
