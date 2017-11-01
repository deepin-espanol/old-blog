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
Este es un aporte para conseguir las credenciales del usuario y de administrador. Recuerda que la contraseña es indispensable para iniciar sesión. Si quieres evitar que intrusos accedan a Deepin, tienes esta opción.

## Cambiar la contraseña de usuario la terminal
1. Ejecuta el comando `sudo passwd [nombre de usuario]`
2. Aparecerá `Enter new UNIX password:`, escribe la nueva contraseña
3. Confirma la contraseña
4. Ya está lista

## Conseguir las credenciales root
1. Desde el GRUB, aparece la ruta: `linux /boot/vmlinuz-3.2.0-18-generic root=UUID=b8b64ed1-ae94-43c6-92\d2-a19dfd9a727e ro recovery nomodeset:`
2. Reemplazar de `recovery nomodeset:” por “rw init=/bin/bash:`
3. Al iniciar en una especie de terminal, escribimos `/usr/sbin/usermod -p [contraseñaderoot] [root]`

## Evitar recuperar las credenciales root
Tienes cuatro formas:
* Añadir protección por contraseña al GRUB.
* Configurar la BIOS y proteger por contraseña.
* Cifrar el disco duro para impedir iniciar el sistema operativo.
* Gestionar los permisos de superusuario a otra cuenta

Recuerda que esos métodos son medidas drásticas. Y eso puede ocurrir:
* Si borras la GRUB no conocerás la ruta de acceso al sistema operativo (en consecuencia tendrías un Kernel panic).
* Si desbloqueas la BIOS, tendrás que configurar desde cero.
* Si quieres descifrar el disco duro, hazlo con generadores de fuerza bruta, una contraseña bien elaborada demora años.
* Cambiar permisos de otra cuenta requiere experiencia.

## Fuente
* [LinuxZone](https://linuxzone.es/faq/%C2%BFcomo-poner-y-recuperar-la-contrasena-de-administrador/)


## Lectura adicional
* [Dudas sobre la terminal]({{ site.url }}{{ site.baseurl }}/anexos/dudas-terminal/).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
