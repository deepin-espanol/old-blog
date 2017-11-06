---
layout: page
title:  "Formas de instalar Deepin"
subheadline:  "Manual"
teaser: "Seamos creativos"
sidebar: right
breadcrumb: true
categories:
    - manual
tags:
    - instalacion
    - pc
    - usb
    - sistemas
    - videos

---
Además de [la instalación convencional]({{ site.url }}{{ site.baseurl }}/instalacion/), te mostramos algunos ejemplos para instalar Deepin.

## Instalación básica

1. Arranca desde el disco o USB: Si no puedes arrancar revisa los ajustes de la BIOS.
2. Sigue las instrucciones: Cómo el idioma o la distribución del teclado.
3. Selecciona la partición a instalar: Opcionalmente puedes establecer el arranque o
4. La instalación demora unos minutos.

## Instalación avanzada
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>

La instalación avanzada ofrece un editor de particiones del disco. Eso es útil para definir que **particiones se conservan o no** como mantener un segundo sistema operativo. Nuestra recomendación es establecer las particiones de arranque y de información como explicamos:

1. Añade una partición EXT4 con el arranque "/" para el sistema operativo. El mínimo es 10GB.
2. Tienes dos formas de establecer el sistema arranque, en el disco duro o en una la partición EXT4 de 300MB "/boot" (para el dual boot).
2. Otra partición "/home" para la carpeta de Mis documentos. Si establecer en un disco duro aparte de los componentes, mejor.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/-oswVXK8Vs0" frameborder="0" allowfullscreen></iframe>
</div>

Fuente: Salmorejo Geek

### Instalación junto a Windows

Si te complica instalar Deepin con la instalación avanzada Deepin con la [aplicación para Microsoft Windows]({{ site.url }}{{ site.baseurl }}/apps/deepininstaller/).

### Deepin en discos externos

Mediante la instalación avanzada, es posible instalar Deepin en discos duros externos o lápices con gran almacenamiento, a partir de 16 GB y completamente en blanco. Los pasos son similares a la dual boot, aunque requiere un puerto de alta velocidad (USB 3.0) para reducir la carga al guardar información.

Para instalar, el dispositivo de arranque debe conectarse en otro puerto.

<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/Ud9aW_L67mQ" frameborder="0" allowfullscreen></iframe>
</div>

{% include alert success='¿Sabes alguna forma de instalar Deepin? ¡contáctanos desde el menú Nosotros!' %}

### Más en Manual
{: .t60 }
{% include list-posts category='manual' entries='3'%}
