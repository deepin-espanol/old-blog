---
layout: page
title:  "Instalar el controlador NVidia desde su ejecutable"
subheadline:  "Tips "
teaser: "Una referencia para instalar archivos desde su sitio web"
categories:
    - tips
tags:
    - controlador
    - driver
    - instalacion

---
Este es un apunte de septiembre de 2017 en que Carlos explica como instalar un ejecutable de Nvidia en la PC. Los pasos resultan liosos e inefectivos en algunas [tarjetas gráficas]({{ site.url }}/manual/videocard/).

## Explicación
Bueno hoy les vengo a enseñar el proceso para instalar el driver Nvidia Oficial usando el Prompt ([del TTY](({{ site.url }}/tips/tty), claro).

1. Descarga el archivo seleccionando su modelo en la [lista de NVidia](http://www.nvidia.es/Download/index.aspx?lang=es). El sistema operativo es Linux y la arquitectura de 32 ó 64 bits, según el caso.

2. Una vez descargado tenemos que desintalar el driver libre Nouveau que trae el sistema por defecto.
  - Para ello presionamos Ctrl+Alt+F1 e ingresamos con nuestra cuenta normal.
  - Luego nos registramos como super usuarios con el comando su y colocando nuestra clave root.
  - Una ves que el Prompt aparezca un simbolo de ´#´, procedemos a detener el servidor de las X con el comando: ´service lightdm stop´
  - Procederemos a desintalar el driver por defecto con ´apt-get —purge remove xserver-xorg-video-nouveau´
  - Y luego reiniciamos con ´reboot´

3. Una vez reiniciado cargara el sistema en modo texto, con una resolucion baja, y presionaremos de nuevo Ctrl+Alt+f1. Ingresamos con nuestra cuenta normal y después como super usuarios con el comando su y colocando nuestra clave root hasta que el Prompt aparezca el símbolo ´#´.
  - Nos moveremos al lugar donde se descargo el archivo que por lo general es en descargas: ´cd Descargas/´
  - Y luego daremos permisos de ejecución al archivo que descargamos con: ´chmod +x NVIDIA-Linux-ARQ-XXX.XX.run´
  - En mi caso el archivo que descargue se llama asi: NVIDIA-Linux-x86-346.47.run
 - Ya aplicado el comando chmod procedemos a detener el servidor de las X con el comando: ´service lightdm stop´
 - Y luego instalar el driver que queremos esto lo hacemos ejecutando el archivo con el comando: ´./NVIDIA-Linux-x86-346.47.run´
 - seguimos los pasos aceptamos todo y listo
iniciamos nuevamente nuestro servidor de las X con:
´service lightdm start´
- Y la instalación está lista.

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
