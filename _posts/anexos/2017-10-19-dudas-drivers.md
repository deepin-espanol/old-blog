---
layout: page-fullwidth
title: "Dudas sobre los contradores en Deepin"
teaser: "Ayudando a probar los dispositivos de la PC"
categories:
    - anexos
tags:
    - dudas
    - driver
    - controladores
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

En esta página respondemos las dudas relacionadas a los controladores en Deepin, en idiomas inglés **drivers**. Es un complemento a la página [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/anexos/dudas/) y [Dudas técnicas]({{ site.url }}{{ site.baseurl }}/anexos/dudas-tecnicas/).

{% include alert success='Esta guía forma parte de una <a href="/dudas">serie de dudas frecuentes</a> para facilitar la comprensión a todos los usuarios y usuarias' %}

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Preámbulo
### ¿Cómo funciona los controladores?
Queremos explicarte cómo funciona Deepin. En el [manual]({{ site.url }}{{ site.baseurl }}/manual/controladores/), explicamos de forma sencillo cómo funciona un controlador

Para comprobar si el dispositivo funciona comprueba si está instalado el módulo dinámico del núcleo o DKMS, algo así como un plugin.

## Preguntas
### ¿Es posible usar el controlador propietario de la tarjeta gráfica?
Sí. Algunos paquetes para optimizar la tarjeta gráfica de NVidia, por ejemplo, está disponible por separado. Visita [está página para conocer los controladores exclusivos disponibles]({{ site.url }}/manual/videocard/).

Si al instalar, no puedes iniciar Deepin, [vuelve a instalar Nouveau]({{ site.url }}/tips/badload-nvidia/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo arreglar la tarjeta inalámbrica o Wifi?
Por defecto, la conexión inalámbrica está actividada en Laptops y dispositivos tipo "rompe muros". Si tienes problemas, [este tip te sirve para encontrar una solución a la conectividad WiFi]({{ site.url }}/tips/wififix/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Es posbile arreglar el Bluetooth? ¿Puedo compartir archivos?
El Bluetooth es un estándar para transferir datos de forma inalámbrica. Basta instalar los paquetes `Bluetooth`, `bluez` y `pulse-audio` (para los audífonos).

Si tienes problemas con la interfaz gráfica, prueba con `blueman` de GNOME.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Existen parches para los microprocesadores?
Microcode es un controlador que aplica parches de rendimiento a los microprocesadores. En general, existen parches para AMD e Intel.

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo arreglar el audio de Deepin?
En Deepin 15.4 se usa [ALSA](https://www.alsa-project.org/main/index.php/Main_Page) (acrónomo de "Advanced Linux Sound Architecture"). Para solucionarlo, [tienes una página con varias opciones]({{ site.url }}/tips/fix-audio/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Cómo configuro la impresora?
Con la aplicación Configuración de impresión (llamada `system-config-printer`). Si quieres conocer la impresora [encontrarás en este manual]({{ site.url }}{{ site.baseurl }}/manual/impresion/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### ¿Puedo cambiar el núcleo de Linux para que mi equipo funcione mejor?
Sí. Esta opción debes considerar como último recurso. Los detalles [encontrarás en el tip]({{ site.url }}{{ site.baseurl }}/tips/kernel/).

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Recursos adicionales
* [Lista de portales de consulta](https://www.linux-drivers.org/) por linux-drivers.
* [Linux Hardware](https://linux-hardware.org/)
* [h.node](https://h-node.org/home/index/es)

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Seguimos creciendo
Si aún no encuentras tu pregunta, usa el [Buscador]({{ site.url }}{{ site.baseurl }}/search/).

No olvides que estamos en [en Github](https://github.com/comunidad-deepin/comunidad-deepin.github.io).

{% include _improve_content.html %}

</div><!-- /.medium-8.columns -->
</div><!-- /.row -->
