---
layout: page
title:  "Arreglar los problemas con la configuración de paquetes"
subheadline:  "Tips "
teaser: "Arreglando tu equipo de la forma fácil"
categories:
    - tips
tags:
    - paquetes
    - configuracion
    - dependencias
    - destacado
---
Si tienes varios problemas con la configuración de Deepin, culpa de la mala actualización o instalación de los paquetes, te proponemos algunas acciones para corregirla sin tener que reinstalar el sistema operativo.

***Aclaración***: Esta página está pensada en realizar en la terminal o en entornos de esritorio de solo texto (Crtl+Alt+F2).

## Volver a actualizar paquetes
Una buena forma es cancelar el resto de actualizaciones de paquetes. Regresar a la versión anterior y volver a actualizar.
~~~
sudo apt-get install --reinstall [nombre del paquete]
~~~

Necesitarás de conexión a Internet para ese prodecimiento.

## Reconfigurar paquetes
Si por equivocación has querido conservar la configuración y encuentras errores con la nueva actualización, intenta ajustar a los valores predeterminados.
~~~
sudo dpkg-reconfigure [nombre del paquete]
~~~

Por ejemplo, para reajustar la [configuración del teclado]({{ site.url }}{{ site.baseurl }}/manual/teclado) tras la actualización, ejecuta.
~~~
sudo dpkg-reconfigure keyboard-configuration
~~~

## Sobre los archivos de configuración
Algunos paquetes tienen una página de configuración temporal almacenada en ´/var/lib/ucf/cache´. Si quieres revisar los cambios entre paquete anterior y renovado, consulta en los foros del proveedor.

## Lectura adicional
* [AskUbuntu](https://askubuntu.com/questions/799212/how-can-i-install-view-the-grub-file-that-a-recent-upgrade-was-providing-but-i-a/799220#799220)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
