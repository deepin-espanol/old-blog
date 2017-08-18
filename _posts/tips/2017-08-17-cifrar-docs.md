---
layout: page
#
# Content
#
subheadline: "Tip"
title: "Cifar mis documentos"
teaser: "La forma más práctica"
categories:
  - tips
tags:
  - cifrar
 
---

{% include alert warning='Si desconoces los pasos de la terminal, pide ayuda a un experto de la materia en el grupo que prefieras.' %}

Para cifrar tus documentos, te ofrecemos los siguientes pasos:

## Requisitos

* Instala el paquete:
{% include alert terminal='sudo apt-get install ecryptfs-utils' %}

* Guarda tus documentos (Home) en otra unidad de disco USB para que la carga sea menor.

## Procedimiento

* Carga el módulo

{% include alert terminal='sudo modprobe ecryptfs' %}

* Crea una nueva cuenta de usuario temporal. Desde el centro de control>Cuentas
* Cierra sesión en tu cuenta (recuerda el nombre) e inicia en la otra

* Ejecuta desde la terminal, siendo <username> el nombre de usuario

{% include alert terminal='ecryptfs-migrate-home -u <username>
' %}

* Una vez que está cifrado la carpeta documentos, ejecuta ´ecryptfs-unwrap-passphrase´ para conseguir la clave de recuperación.
* Es todo, sal y elimina la cuenta de usuario temporal 
* Reinicia el equipo
* Ahora está listo

### Crédito

* [Wiki de Debian](https://wiki.debian.org/TransparentEncryptionForHomeFolder)