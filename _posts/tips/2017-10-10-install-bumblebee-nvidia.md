---
layout: page
title:  "Instalar Nvidia Bumblebee"
subheadline:  "Tips "
teaser: "Un controlador para laptops con dicha marca de video"
categories:
    - tips
tags:
    - nvidia
    - Bumblebee
    - controlador

---
Este es un apunte de septiembre de 2017 en que Carlos explica como instalar un ejecutable de Nvidia en la PC. Los pasos resultan liosos e inefectivos en algunas [tarjetas gráficas]({{ site.url }}/manual/videocard/).

## Instalación
Bueno hoy les vengo a enseñar el proceso para instalar el componentes Bumblebee de Nvidia usando el Prompt (de la [TTY]({{ site.url }}/manual/tips/tty/), claro).

1. $ sudo apt install mesa-utils inxi
2. $ sudo apt install xserver-xorg-input-mouse
3. Instalar desde [sourceforge](https://sourceforge.net/projects/virtualgl/files/2.5.2/virtualgl_2.5.2_amd64.deb/download)
4. Aplicar $ sudo apt-get install nvidia-kernel-dkms nvidia-xconfig nvidia-settings nvidia-vdpau-driver vdpau-va-driver
5. $ sudo apt install bumblebee (acepta todo hasta finalizar el paso)
6. $ sudo adduser "name user" bumblebee (sin las comillas, es el nombre de usuario)
7. $ sudo service bumblebeed (reiniciar)
8. Otra vez reiniciar


## Otros detalles
### Probar Bumblebee
1. $ glxgears
2. $ optirun glxgears
3. $ inxi -Gx
4. $ optirun inxi -Gx

### Configuración
Configurar Nvidia-Settings
1. ´$ cd /usr/share/applications´
2. ´$ sudo gedit nvidia-settings.desktop´
3. Modificar la linea "Exec" por ´Exec=optirun nvidia-settings -c :8.0´
4. Guardar

### Configurar aplicaciones que requieran la aceleración 3D
1. $ cd /usr/share/applications
2. $ dir
Buscar “applicaion”.desktop y modificar la línea que diga "Exec" y añade “optirun” una línea antes de este
  - $ sudo gedit blender.desktop
3. Cambiar Exec=blender por Exec=optirun blender

### Configurar juegos Steam
1. Abrir Steam
2. En el Apartado “Biblioteca”, señalar el juego que queramos que arranque con aceleración 3d de Nvidia, pulsar botón derecho del ratón y señalar “propiedades”
3. En la pestaña “general", clic en el botón “Definir parámetros de lanzamiento”.
4. Y en el cuadro rellenar con: primusrun %command%

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
