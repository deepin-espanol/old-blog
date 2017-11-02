---
layout: page
title:  "Gestionar permisos de usuario"
subheadline:  "Tips "
teaser: "Quiénes pueden modificar el equipo, para impedir instrusos"
breadcrumb: true
categories:
    - tips
tags:
    - root
    - password
    - acceso
---
Este es un aporte para cambiar las credenciales del usuario y de administrador. Recuerda que la contraseña es indispensable para iniciar sesión. Si quieres evitar que intrusos accedan a Deepin, tienes esta opción.

## Mediante GNOME System Tools
Visita [Usar GNOME System Tools]({{ site.url }}{{ site.baseurl }}/tips/gnome-system-tools/).

## Mediante la terminal
Para conceder al otro usuario los permisos de superadministrador:
1. Ejecuta `sudo visudo`, tendrás el archivo `sudoers`
2. Ir a la línea `root    ALL=(ALL:ALL) ALL`
3. Escribir una nueva línea de esta manera `[nombre usuario]    ALL=(ALL:ALL) ALL`

## Fuente
* [Slimbook](https://slimbook.es/tutoriales/linux/86-anadir-usuario-al-fichero-sudoers)


## Lectura adicional
* [Dudas sobre la terminal]({{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
