---
layout: page
title:  "Conflcitos con la configuración en nuevos paquetes"
subheadline:  "Tips "
teaser: "Solucionando el problema de cambiar los paquetes actualizados"
breadcrumb: true
categories:
    - tips
tags:
    - paquetes
    - configuracion
    - dependencias
    - destacado
---
Al actualizar Deepin, la configuración los paquetes se renueva para adaptarse con sus versiones mejoradas. En esta página te enseñamos que hacer frente a los cambios, sobre todo si lo realizas en la terminal.

## Porqué aparecen esos avisos
Al realizar una actualización mayor, se cambian los componentes críticos del sistema como el sistema de apagado, el teclado, el núcleo, entre otros.

Cada paquete tiene una configuración (archivo ´conf´) que puedes modificarlo en el centro de control o un aplicación del sistema. Sin embargo, al conseguir la última versión, tenemos la posibilidad de realizar modificaciones necesarias para que el sistema operativo funcione apropiademente.

<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}conf-terminal.png" alt="Aplicación Aptitude.">
    </div>
</div>


<div class="row">
    <div class="medium-12 columns t30">
    <img src="{{ site.urlimg }}conf-terminal2.png" alt="Aplicación Aptitude.">
    </div>
</div>

## Solución

Antes de actualizar, asegúrate de realizar correctamente esos comandos, evitando problemas por falta de dependencias y similares.
~~~
sudo apt update
sudo apt-get check
sudo apt full-upgrade
~~~

Cuando estás actualizando, aparecerá un aviso en modo texto o mediante botones. Este es un ejemplo de un paquete a mejorar.

~~~
Fichero de configuración `/etc/xxxx.d/xxxx.conf'
El proveedor del paquete ofrece una nueva configuración lista para su funcionamiento.
Sin embargo, debido a que la configuración fue alterada, requiere tomar una decisión:
(1) Cambiar la configuración del proveedor
(2) Conservar los cambios de la configuración
(3) Ver los cambios de ambas configuración
(4) Revisar el código fuente de los archivos
~~~

Recomendamos realizar la primera opción o similares y pulsar Enter. En algunos casos, son expresados en letras de confirmación (como Y).

### Para diálogos en inglés
Anteriormente mostramos una traducción aproximada. Aquí dejamos una referencia en el idioma original (inglés). Puede resultar útil para consultar a los dearrolladores o en un foro internacional:

~~~
A new version of configuration file `/etc/xxxx.d/xxxx.conf' is available, but the version installed currently has been locally modified:
(1) Install the package maintainer's version
(2) Keep the local version currently installed
(3) Show the differences between the versions
(4) Show a side-by-side difference between the versions
~~~

## Recuperar valores predeterminados
Si por error has conservado la configuración después de que los paquetes fueran actualizados, revisa [esta página]({{ site.url }}{{ site.baseurl }}/tips-problemas-conf-paquete).

## Lectura adicional
* [Archivo en la lista de Ubuntu Argentina](https://lists.ubuntu.com/archives/ubuntu-ar/2009-July/022299.html)
* [Consulta en stackexchange ](https://unix.stackexchange.com/questions/113732/a-new-version-of-configuration-file-etc-default-grub-is-available-but-the-vers)
* [AskUbuntu](https://askubuntu.com/questions/799212/how-can-i-install-view-the-grub-file-that-a-recent-upgrade-was-providing-but-i-a/799220#799220)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
