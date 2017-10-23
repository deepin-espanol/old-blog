---
layout: page
title:  "Abrir archivos y montar unidades desde la terminal"
subheadline:  "Tips "
teaser: "Usando 'cd' para ver las carpetas y otros trucos"
categories:
    - tips
tags:
    - terminal
    - cd
    - archivos
---
Al abrir la terminal o [estar modo TTY]({{ site.url }}{{ site.baseurl }}/tips/tty/), usa el comando `cd` como reemplazo temporal al explorador. También aprenderás a montar (comando `mount`) unidades de almacenamiento externo.

Si quieres saber más detalles sobre esté y la terminal Deepin visita [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/tips/dudas-terminal/).

## Acciones básicas
### Abrir archivos y explorar carpetas
Como no tendrás el gestor de archivos de forma gráfica, prueba con `cd`:
~~~
cd /[nombre de la carpeta]/
~~~

Ir atrás

~~~
cd..
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Lista de archivos
Si quieres conocer los archivos que encontramos en la carpeta recurrimos al `ls`:

~~~
ls -l
~~~

Para ver el tipo de archivo, usamos en su lugar:

~~~
ls -F
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Leer archivos de sólo textos
Para ver el contenido del archivo recurrimos a `more`. Sin embargo, lo que veremos es sólo el texto sin formato. También es útil para conocer lo hay adentro del archivo como "ejecutables"  antes de instalar.

Las opciones para leer el archivo tenemos `more` para mostrar de arriba y abajo, `head` para ir al inicio y `tail` para el final:

~~~
more archivo
head archivo
head -20 archivo
tail archivo
tail -20 archivo
~~~
<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Copiar y mover archivos
Para copiar y mover archivos usamos `cp` y `mv`. Por ejemplo, si quiero mover `archivo.txt` a `/home/datos/` hacemos lo siguiente:

~~~
cp archivo.txt /home/datos/
mv archivo.txt /home/datos/
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Borrar archivo
{% include alert alert='¡No podrás recuerar archivos una vez borrados! Asegúrate escrbir el nombre del archivo correctamente.' %}
Para borrar archivos escribimos el temido `rm`:

~~~
rm [nombre del archivo]
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

## Unidades externas
### Montar el dispositivo USB
1. Si quieres abrir el dispositivo USB (flash, memoria) tenemos que localizar la partición y crear la unidad `/media/usb`

~~~
mkdir /media/usb
ls -l /dev/sd*
~~~

2. Para montar usamos el comando `mount` y escribimos lo siguiente, teniendo en cuenta que la partición del usb en el ejemplo es `/dev/sdb1` y tipo de formato es `vfat` para FAT (o `ntfs` para NTFS):

~~~
mount -t vfat /dev/sdb1 /media/usb
~~~

3. Ahora vayamos a la unidad el USB, para buscar el archivo seguimos con `cd`

~~~
ls /media/usb
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }

### Cambiar permisos de lectura y escritura

Para cambiar los permisos recurrimos a esta opción:

~~~
sudo mount / -o remount,rw
~~~

<small markdown="1">[Ir al índice](#toc)</small>
{: .text-right }


## Lectura adicional
* [Geekland](https://web.archive.org/web/20161122185103/https://geekland.eu/montar-la-memoria-usb-en-la-terminal/)
* [Blog "Principiante Blog"](http://principiante-linux.blogspot.pe/2007/08/comandos-linux-mover-copiar-borrar-y.html)
* [Soluciones al cargar Deepin]({{ site.url }}{{ site.baseurl }}/anexos/badload/)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
