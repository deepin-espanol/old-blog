---
layout: page
title:  "Instalar otros entornos de escritorio"
subheadline:  "Tips "
teaser: "Una referencia para probar otros entornos de escritorio en Deepin"
categories:
    - tips
tags:
    - pruebas
    - entorno
    - escritorio
---
Si quieres probar otros entornos de escritorios como KDE o GNOME, incorporamos un listado de paquetes a instalar.

## Lista de entornos de escritorio disponibles
### Budgie Descktop
~~~
sudo apt install budgie-desktop && budgie-core && budgie-indicator-applet && budgie-dock && nautilus && nautilus-admin && nautilus-open-terminal && nautilus-gtkhash && nautilus-hide && gnome-tweack-tool && plank && totem
~~~
### Cinnamon Desktop
~~~
sudo apt install cinnamon && cinnamon-core && cinnamon-doc && nemo && nemo-gtkhash && nemo-python && plank && totem    
~~~
### Genome Shell
~~~
sudo apt install gnome-shell && gnome-shell-extensions && gnome-shell-extension-weather && gnome session && nautilus && nautilus-admin && nautilus-open-terminal && nautilus-gtkhash && nautilus-hide && gnome-tweack-tool && totem
~~~
### Plasma Desktop (KDE)
~~~
sudo apt install plasma-desktop && dolphin && dolphin-plugins && ffmpegthumbs && gdebi-kde
~~~
### Mate Desktop
~~~
sudo apt install mate-desktop-environment && mate-applet-brisk-menu && caja-actions && caja-extensions-common && caja-gtkhash && caja-open-terminal && caja-wallpapers && mate-utils && mate-tweack
~~~
### Xfce Desktop
~~~
Sudo apt install xfce4 && xfce4-whiskermenu-plugin && xfce4-weather-plugin && xfce4-volumed-pulse && thunar-vcs-plugins && thunar-media-tags-plugin && thunar-gtkhash
~~~
### Lxde Desktop
~~~
sudo apt install lxde && lxpanel-top-menu
~~~

## Notas

* Es posible que al instalar un paquete del entorno, se muestra en otros más.

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
