---
layout: page-fullwidth
title: "Actualización"
subheadline: "Sistema operativo"
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
## Recomendaciones

Antes de actualizar Deepin tu equipo debe estar preparado:

* Ten al menos 10 GB de espacio libre en el disco duro o sólido para descargar los archivos
* Tu equipo debe estar conectado a Internet, cableado o vía WiFi
* Cierra las aplicaciones que consuman muchos recursos
* En caso de computadores portátiles, debe tener un buen estado de batería

### Selecciona un espejo

Aparte del [oficial](https://www.deepin.org/en/mirrors/packages/):

1. Dígete al Centro de Control
2. Selecciona "Actualizar"
3. Escoge un espejo haciendo una prueba
4. Selecciona el espejo más rápido

Ejemplos:
* [Linux Kernel Mirror](http://mirrors.kernel.org/deepin/)
* [Silicon Valley](http://mirror1.sjc02.svwh.net/deepin/)
* Otros espejos en [la página Lista de espejos]({{ site.url }}//tips/mirror/).

## Actualizar

La forma más elegante de conseguir la última versión es accediendo al Centro de Control.

1. Revisa si tienes una notificación o dirígete a la opción "Actualizar";
2. Espera unos minutos, dependiendo de la conexión a Internet;
3. Revisa la lista de cambios y haz clic en actualizar;
4. Cuando se descarga los componentes del sistema, cierra las aplicaciones y procede a instalar;
5. Se reiniciará y demorará unos minutos.

## Anexos

### Ver los útlimos cambios
Tenemos un listado de cambios en la opción "Revisa las novedades". Para las actualizaciones de seguridad visita la [página web de Deepin](https://www.deepin.org/en/category/system-update/).

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/novedades/">No olvides revisar las novedades y avances ›</a>

## Usar la terminal
Otra forma es accediendo a la **Terminal de Deepin**, útil para no reiniciar el equipo o comprobar las dependencias en los paquetes. En primer lugar, deberás actualizar la lista de paquetes con el comando `update` y escribe la contraseña root.

Más detalles en [la página correspondiente]({{ site.url }}/tips/sources/).

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
