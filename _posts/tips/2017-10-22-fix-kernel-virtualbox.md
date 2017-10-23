---
layout: page
title:  "Corregir problema del kernel de VirtualBox"
subheadline:  "Tips "
teaser: "Extaído del foro de Deepin"
breadcrumb: true
categories:
    - tips
tags:
    - driver
    - nvidia
    - boot
---
En esta página te enseñamos a corregir un error en el núcleo de [VirtualBox]({{ site.url }}{{ site.baseurl }}/apps/virtualbox/). Está relacionado con la instalación de Windows 10 en Deepin OS.

~~~
The VirtualBox Linux kernel driver (vboxdrv) is either not loaded or there is a permission problem with /dev/vboxdrv. Please install virtualbox-dkms package and load the kernel module by executing.
~~~

## Pasos

Realizamos estas actividades desde la terminal, instalando el paquete `virtualfox-dkms` y modificando el núcleo:

~~~
sudo usermod -G vboxusers -a root
sudo apt-get install linux-headers-`uname -r`
sudo apt-get install virtualbox-dkms
sudo dpkg-reconfigure virtualbox-dkms
sudo modprobe vboxdrv
~~~

## Lectura adicional
* [Foro de Deepin](https://bbs.deepin.org/forum.php?mod=viewthread&tid=37873)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
