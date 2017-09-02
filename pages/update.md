---
layout: page-fullwidth
title: "Actualización"
subheadline: "Actualiza Deepin fácilmente"
teaser: "Los pasos más claros para actualizar"
permalink: "/update/"
header:
   image_fullwidth: "wallpaper.jpg"
---
<div class="row">
<div class="medium-4 medium-push-8 columns" markdown="1">
<div class="panel radius" markdown="1">
**Table of Contents**
{: #toc }
*  TOC
{:toc}
</div>
</div><!-- /.medium-4.columns -->

<div class="medium-8 medium-pull-4 columns" markdown="1">
{% include _improve_content.html %}

## Antes de actualizar

Antes de actualizar Deepin tu equipo debe estar preparado:

* Ten al menos 10 GB de espacio libre en el disco duro o sólido para descargar los archivos
* Tu equipo debe estar conectado a Internet
* Evita ejecutar aplicaciones pesadas o que comprometa el rendimiento del equipo

## Selecciona un espejo

Aparte del [oficial](https://www.deepin.org/en/mirrors/packages/):

1. Dígete al Centro de Control
2. Selecciona "Actualizar"
3. Escoge un espejo haciendo una prueba
4. Selecciona el espejo más rápido

Ejemplos:
* [Linux Kernel Mirror](http://mirrors.kernel.org/deepin/)
* [Silicon Valley](http://mirror1.sjc02.svwh.net/deepin/)

## Actualizar

La forma más elegante de actualizar, es accediendo el acceso "Actualizar" desde el Centro de Control.

### Pasos

1. Actualiza 
2. Espera unos minutos, dependiendo de la conexión a Internet
3. Haz clic en actualizar
4. Cuando se actualiza componentes del sistema, cierra las aplicaciones y procede
5. Se reiniciará y demorará unos minutos

## Anexo: Desde la terminal
Otra forma es accediendo a la **Terminal de Deepin**, útil para no reiniciar el equipo. En primer lugar, deberás actualizar la lista de paquetes con el comando `update` y escribe la contraseña root.

~~~
sudo apt update
~~~

Continúa ejecute este comando:

~~~
sudo apt upgrade && sudo apt full-upgrade
~~~

Tardará unos minutos, mientras ves los detalles en la ventana. Considera que ´upgrade´ significa "mejorar" y `full-upgrade` es para cambiar de versión (digamos de 15.3 a 15.4).

{% include alert success='Quieres mejorar, ¡colabora con nosotros!' %}
{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
