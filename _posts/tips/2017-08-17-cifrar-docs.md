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

1. Carga el módulo, que se añadirá en la lista de arranque

{% include alert terminal='sudo modprobe ecryptfs' %}

2. Crea una nueva cuenta de usuario temporal. Desde el "Centro de control>Cuentas"
3. Cierra sesión en tu cuenta (recuerda el nombre) e inicia en la otra
4. Ejecuta desde la terminal, siendo username el nombre de usuario

{% include alert terminal='ecryptfs-migrate-home -u username
' %}

5. Una vez que está cifrado la carpeta documentos, ejecuta ´ecryptfs-unwrap-passphrase´ para conseguir la clave de recuperación.
6. Además tienes una carpeta Home con los archivos sin cifrar. Si deseas muévelo o bórralo
7. Reinicia el equipo
8. Inicia sesión con la cuenta de usuario habitual y elimina la temporal
9. Ahora está listo para usar

Nota: Otro método es realizar sin abrir el entorno de escritorio en lugar de crear una cuenta de usuario temporal.

Nota 2: También puedes cifrar la partición SWAP con sudo apt-get install cryptsetup y sudo ecryptfs-setup-swap. No recomendamos seguir esta opción porque podría interfierir el rendimiento de la memoria RAM:

### Crédito

* [Wiki de Debian](https://wiki.debian.org/TransparentEncryptionForHomeFolder)
* [Página web de eCryptfs](http://ecryptfs.org)