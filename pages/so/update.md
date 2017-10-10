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

## Recomendaciones

Antes de actualizar Deepin tu equipo debe estar preparado:

* Ten al menos 10 GB de espacio libre en el disco duro o sólido para descargar los archivos;
* Tu equipo debe estar conectado a Internet, cableado o vía WiFi;
* Cierra las aplicaciones que consuman muchos recursos;
* En caso de computadores portátiles, debe tener un buen estado de batería.

### Selecciona un respositorio

Aparte del [oficial](https://www.deepin.org/en/mirrors/packages/) tienes una serie de repositorios optimizados para descargar:

1. Dígete al Centro de Control
2. Selecciona "Actualizar"
3. Escoge un espejo haciendo una prueba
4. Selecciona el espejo más rápido

Ejemplos:
* [Linux Kernel Mirror](http://mirrors.kernel.org/deepin/)
* [Silicon Valley](http://mirror1.sjc02.svwh.net/deepin/)
* Otros espejos en [la página Lista de espejos]({{ site.url }}{{ site.baseurl }}/tips/mirror/).

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/manual/espejos/">Información sobre los espejos ›</a>

## Realizar una actualización

La forma más elegante de conseguir la última versión es accediendo al Centro de Control.

1. Revisa si tienes una notificación o dirígete a la opción "Actualizar";
2. Espera unos minutos, dependiendo de la conexión a Internet;
3. Revisa la lista de cambios y haz clic en actualizar;
4. Cuando se descarga los componentes del sistema, cierra las aplicaciones y procede a instalar;
5. Se reiniciará y demorará unos minutos.

Para saber cómo funciona y cómo aprovechar las actualizaciones, visita [la página Espejos]({{ site.url }}{{ site.baseurl }}/manual/espejos/). En caso de tener problemas, prueba a editar el archivo que te explicaremos en [la página correspondiente]({{ site.url }}{{ site.baseurl }}/tips/sources/).

Al encontrarte con avisos tipo "El distribuidor del paquete ha publicado un archivo de configuración actualizado", o similar, revisa la página [Solución a las actualizaciones de configuración]({{ site.url }}{{ site.baseurl }}/tips/actualizar-conf-paquetes/).

## Ver los útlimos cambios
Tenemos un listado de cambios en la opción "Revisa las novedades". Para las actualizaciones de seguridad visita la [página web de Deepin](https://www.deepin.org/en/category/system-update/).

<a class="radius button small" href="{{ site.url }}{{ site.baseurl }}/novedades/">No olvides revisar las novedades y avances ›</a>

{% include alert success='Quieres mejorar, ¡colabora con nosotros!' %}
{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
