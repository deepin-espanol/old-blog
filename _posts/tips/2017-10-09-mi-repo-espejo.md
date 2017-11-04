---
layout: page
title:  "Elaborar un repositorio espejo"
subheadline:  "Tips "
teaser: "Consigue una copia del repositorio Deepin para proveer a otros usuarios"
breadcrumb: true
categories:
    - tips
tags:
    - repositorio
    - espejo
    - instalacion

---
Los repositorios son indispensables para Deepin. Contienen los componentes necesarios para instalar aplicaciones y actualizar el equipo. Tenemos [un listado según el lugar que residas]({{ site.url }}/manual/espejos/).

En está página te explicamos como elaborar uno propio para uso particular o público. Cabe señalar, que no es para las computadoras sino para servidores con gran ancho de banda para ese fín. Si brindas muchísimo ancho de banda puedes colaborar con la lista oficial de Deepin.

## Requisitos
Los requisitos son flexibles. El servidor debe ser GNU/Linux operativo, con una buena capacidad de almacenamiento y capacidad de procesar varias peticiones por segundo. La seguridad HTTPS es recomendada para mejor seguridad.

La sincronización con los repositorios de China se muestra en la siguiente tabla:

<table>
  <caption>Sincronización con los repositorios</caption>
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
      <td>Repositorio de paquetes</td>
      <td>275GB a más</td>
    </tr>
    <tr>
      <td>Repositorio de ISO</td>
      <td>50 GB a más</td>
    </tr>
    <tr>
      <td>Recomendado</td>
      <td>400 GB a más</td>
    </tr>
  </tbody>
</table>

Nota: Otras características para mejorar la estabilidad son a criterio de cada uno.

## Pasos
1. Establece el dominio web como repositorio solo para Deepin
   - Ejemplo: `https://deepin.mirepositor.io`
2. Instala `rsync`
   - Desde la terminal: `sudo apt install rsync`
3. Ejecuta `rsync` para sincronizar los respositorios
  - rsync -av –delete-after rsync.deepin.com::deepin/ /var/www/deepin/
  - rsync -av –delete-after rsync.deepin.com::releases/ /var/www/deepin-cd/
4. Para automitizar el proceso recomendamos usar el proceso ´Cron Job´.
5. No añadas otros paquetes al espejo. Para eso usa repositorios aparte.

## Lectura adicional
* Si deseas cooperar con la lista de espejos recomendados para Deepin, envia un mensaje a support@deepin.org (en inglés).

### Más en Tips
{: .t60 }
{% include list-posts category='tips' entries='3'%}
