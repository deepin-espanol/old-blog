---
layout: page
title:  "Instalar otros entornos de escritorio"
subheadline:  "Tips "
teaser: "Una referencia para probar otros entornos de escritorio en Deepin"
breadcrumb: true
categories:
    - tips
tags:
    - pruebas
    - entorno
    - escritorio
---
Si quieres probar otros entornos de escritorios como KDE o GNOME, incorporamos un listado de paquetes a instalar.

## Antes de probar
* Recomendamos usar varios escritorios solo a desarrolladores de aplicaciones o a aquellos que aún no se acostumbraron a Deepin.
* Es posible que al instalar un paquete del entorno, se muestre en Deepin y otros más.
* Las aplicaciones de Deepin están escritas en DTK, que se distancia con las escritas en Qt (Plasma) y GTK (Gnome). Irónicamente, DTK utiliza una versión modificada en QT, [qt5integration](https://github.com/linuxdeepin/qt5integration).
* Los paquetes del repositorio de Deepin no están actualizadas en tiempo real, probarlas es bajo tu responsabilidad.

## Lista de entornos de escritorio disponibles
### Budgie Desktop
~~~
sudo apt install budgie-desktop && budgie-core && budgie-indicator-applet && budgie-dock && nautilus && nautilus-admin && nautilus-open-terminal && nautilus-gtkhash && nautilus-hide && gnome-tweack-tool && plank && totem
~~~
Basado en GNOME para el sistema operativo Solus.
### Cinnamon Desktop
~~~
sudo apt install cinnamon && cinnamon-core && cinnamon-doc && nemo && nemo-gtkhash && nemo-python && plank && totem    
~~~
Basado en GNOME v3 para Linux Mint.
### Gnome Shell
~~~
sudo apt install gnome-shell && gnome-shell-extensions && gnome-shell-extension-weather && gnome session && nautilus && nautilus-admin && nautilus-open-terminal && nautilus-gtkhash && nautilus-hide && gnome-tweack-tool && totem
~~~
Entorno desarrollado activamente. Por defeco en Ubuntu (como 18.04).
### Plasma Desktop (KDE)
~~~
sudo apt install plasma-desktop && dolphin && dolphin-plugins && ffmpegthumbs && gdebi-kde
~~~
Entorno desarrollado activamente. Por defecto en OpenSuse, Kubuntu y otras distribuciones.
### Mate Desktop
~~~
sudo apt install mate-desktop-environment && mate-applet-brisk-menu && caja-actions && caja-extensions-common && caja-gtkhash && caja-open-terminal && caja-wallpapers && mate-utils && mate-tweack
~~~
Entorno de escritorio de bajo consumo para Linux Mint.
### Xfce Desktop
~~~
Sudo apt install xfce4 && xfce4-whiskermenu-plugin && xfce4-weather-plugin && xfce4-volumed-pulse && thunar-vcs-plugins && thunar-media-tags-plugin && thunar-gtkhash
~~~
Entorno de escritorio para Puppy Linux. Su integración es limitada como su consumo.
### Lxde Desktop
~~~
sudo apt install lxde && lxpanel-top-menu
~~~
Entorno de escritorio para Puppy Linux de muy bajo consumo, recomendado para la Internet de las cosas.
### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
