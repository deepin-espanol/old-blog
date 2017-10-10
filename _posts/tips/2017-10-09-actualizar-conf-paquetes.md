---
layout: page
title:  "Conflcitos con la configuración en nuevos paquetes"
subheadline:  "Tips "
teaser: "Solucionando el problema de cambiar los paquetes renovados"
categories:
    - tips
tags:
    - paquetes
    - configuracion
    - dependencias

---
Al actualizar Deepin, la configuración los paquetes son editados para adaptarse con sus versiones mejoradas. En esta página te enseñamos que hacer frente a los cambios, sobre todo si lo realizas en la terminal.

## Porqué aparecen esos avisos
Al realizar una actualización mayor, se cambian los componentes críticos del sistema como el sistema de apagado, el teclado, el núcleo, entre otros.

Cada paquete tiene una configuración (archivo ´conf´) que irá cambiando a medida que lo modifiquemos. Sin embargo, los paquetes actualizados ofrecen modificaciones necesarias para que el sistema operaivo funcione apropiademente.

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

## Lectura adicional

* [Archivo en la lista de Ubuntu Argentina](https://lists.ubuntu.com/archives/ubuntu-ar/2009-July/022299.html)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
