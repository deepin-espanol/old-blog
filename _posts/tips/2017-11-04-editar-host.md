---
layout: page
title:  "Recuperar contraseña de usuario"
subheadline:  "Tips "
teaser: "Para quienes no pueden acceder la cuenta de usuario"
breadcrumb: true
categories:
    - tips
tags:
    - root
    - password
    - acceso
---
En Deepin tienes un truco secreto para impedir que ingrese páginas que no cosideras adecuadas con los host, ubicada en `/etc/hosts` del sistema. Si usas algún bloqueador de terceros, esta opción es mucha más eficiente y nativa.

## Detalles
El archivo `host.conf` es el encargado de filtrar las peticiones de los dominios web. Es decir, bloqueará cualquier conexión con la página web o la IP de esta. La línea establecida es `127.0.0.1 localhost` para procesar la conexión local a la red local y `0.0.0.0 wikipedia.org` para rechazar la conexión.

Antes de editar el archivo host, haz una copia de seguridad `sudo cat /etc/hosts.back >> /etc/hosts`.

## Métodos
### Editando el archivo host
1. Ejecutando desde la terminal `sudo nano /etc/hosts`
2. Pegando el código fuente de [Steven Black](https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts)

### Actualizando
La forma más sencilla de editar es:
1. Asegurar tener instalado `cron`
2. Ejecuta `sudo crontab -e` para editar el archivo
3. Añadir la siguiente línea copiando desde ` https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts`

Notas:
* `30 5 */5` es el intervalo de tiempo para actualizar. Empieza con segundos, minutos, horas y días. Puedes generar un propio desde [crontab-generator](https://crontab-generator.org/).
* `wget -0` realiza una edición
* El código a sincronizar, lo extraímos de [Steven Black](https://github.com/StevenBlack/hosts)

## Fuente
* [Lignux](https://lignux.com/bloqueando-toda-la-publicidad-con-el-fichero-hosts/)

## Lectura adicional
* [Dudas técnicas]({{ site.url }}{{ site.baseurl }}/anexos/dudas-tecnicas/).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
