---
layout: page
title:  "Elaborar un repositorio espejo"
subheadline:  "Tips "
teaser: "Consigue una copia del repositorio Deepin para proveer a otros usuarios"
categories:
    - tips
tags:
    - repositorio
    - espejo
    - instalacion

---
Los repositorios proveen los componentes necesarios para instalar y actualizar. Siempre puedes [seleccionar el repositorio según el lugar que residas]({{ site.url }}/manual/espejos/).

En está página te explicamos como elaborar un repositorio. Cabe señalar, que no es para cualquiera sino para empresas que tengan espacio disponible para varios usuarios locales.

## Requisitos
Si bien la capacidad de los servidores es criterio de cada uno, el almacenamiento para sincronizar los repositorios de China son los siguientes.

<table>
  <caption>Requisitos para sincronizar los repositorios</caption>
  <colgroup>
    <col span="1" style="width: 70%;">
    <col span="1" style="width: 30%;">
      </colgroup>
  <thead>
    <tr>
      <th>Instrucción</th>
      <th>Espacio requerido</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>rsync -av –delete-after rsync.deepin.com::deepin/ /var/www/deepin/</td>
      <td>275GB a más</td>
    </tr>
    <tr>
      <td>rsync -av –delete-after rsync.deepin.com::releases/ /var/www/deepin-cd/</td>
      <td>50 GB a más</td>
    </tr>
    <tr>
      <td>Recomendado</td>
      <td>400 GB a más</td>
    </tr>
  </tbody>
</table>

El tiempo para sincronizar los paquetes varía (recomendamos hacer a diario mediante la orden ´cron´). Para evitar problemas, no añadas paquetes personalizados.

## Lectura adicional

* Si deseas cooperar con la lista de espejos recomendados para Deepin, envia un mensaje a support@deepin.org (en inglés).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
