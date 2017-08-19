---
layout: page
#
# Content
#
subheadline: "Tip"
title: "Cifrar mis documentos"
teaser: "La forma más práctica"
categories:
  - tips
tags:
  - cifrar
 
---

{% include alert warning='Si desconoces los pasos de la terminal, pide ayuda a un experto de la materia en el grupo que prefieras.' %}

Existen formas de crear una carpeta para cifrar tus documentos. Estarás más o menos a salvo de intrusos incluyendo un código para que accedas desde otra distro compatible. Te ofrecemos los siguientes pasos:

## Requisitos

* Debes tener el paquete ecryptfs-utils. Desde la termina puedes instalar:
{% include alert terminal='sudo apt-get install ecryptfs-utils' %}

* Necesitarás espacio para que copie la carpeta "Home". Para reducir la carga, mueve tus documentos (Home) en otra unidad de disco USB.

* Esta función no planea cifrar el disco duro para no limitar el rendimiento y arranque del equipo. No obstante, puede consumir un poco de memoria RAM y CPU.

## Procedimiento

1. Carga el módulo, que se añadirá en la lista de arranque;

{% include alert terminal='sudo modprobe ecryptfs' %}

2. Cierra sesión e inicia desde la [terminal virtual]({{ site.url }}/tty/);
3. Ejecuta desde la terminal, siendo username el nombre de usuario;

{% include alert terminal='sudo ecryptfs-migrate-home -u username
' %}

4. Una vez que está cifrado la carpeta documentos, ejecuta ´ecryptfs-unwrap-passphrase´ para conseguir la clave de recuperación y guardarlo en caso que sea necesario;
5. Reinicia el equipo o escribiendo el comando "sudo reboot";
6. Cuando abras el gestor de archivos tendrás dos carpetas Home, la que estás usando y una copia sin cifrar, si deseas muévelo o bórralo;
7. Ahora está listo para usar

### Notas aclaratorias

* Otro método es realizar este proceso es tener una cuenta temporal.
	- Créala desde el "Centro de control>Cuentas"
	- Abre la terminal desde la cuenta temporal y borra dicha cuenta cuando finalices al 100%

* También puedes cifrar la partición SWAP con "sudo apt-get install cryptsetup" y "sudo ecryptfs-setup-swap". No recomendamos seguir esta opción porque podría interfierir el rendimiento de la memoria RAM:

### Crédito

* [Wiki de Debian](https://wiki.debian.org/TransparentEncryptionForHomeFolder)
* [Página web de eCryptfs](http://ecryptfs.org)