---
layout: page
title:  "Configurando systemd con chkservice"
subheadline:  "Tips "
teaser: "Establece los servicios del sistema a tu gusto"
categories:
    - tips
tags:
    - chkservice
    - demonio
    - systemd
---
systemd (acrónomo de "System daemon", escrito en minúsculas) es un conjunto de servicios del sistema, también llamados "demonios", siendo el primero al iniciar del sistema. En este tip te enseñamos a establecer qué servicios puede iniciar a con él gracias a chkservice.

Si quieres saber más detalles sobre esté y más componentes en Deepin , visita [Dudas frecuentes]({{ site.url }}{{ site.baseurl }}/tips/dudas-tecnicas/).

## Pasos
1. Descarga desde los repositorios `apt installchkservice`
chkservice
<div class="flex-video">
        <iframe width="1280" height="720" src="//www.youtube.com/embed/A_VM9XSBaus" frameborder="0" allowfullscreen></iframe>
</div>

## Usar Chekservice sin entorno gráfico

En caso que encuentres un error realcionado a Systemd, puedes iniciar [en modo TTY]({{ site.url }}{{ site.baseurl }}/tips/tty/).

## Lectura adicional
* [Artículo en Linoxide](https://linoxide.com/linux-how-to/chkservice-systemd-units-management/)
* [SystemD en Freedesktop](https://www.freedesktop.org/wiki/Software/systemd/)
* [Artículo de Wikipedia](https://en.wikipedia.org/wiki/Systemd)

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
