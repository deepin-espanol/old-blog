---
#
# Use the widgets beneath and the content will be
# inserted automagically in the webpage. To make
# this work, you have to use › layout: frontpage
#
layout: frontpage
header:
  image_fullwidth: header_unsplash_12.jpg
widget1:
  title: "Instructivo"
  url: 'http://comunidad-deepin.github.io/blog/'
  image: widget-1-302x182.jpg
  text: 'Enseñamos y preparamos a aquellos que quie&shy;ren usar el sistema operativo. <em>Comunidad Deepin</em> ofrece una blog, tutoriales y consejos para todas las necesidades. Si aún tienes nociones básicas sobre computación, te guíaremos.'
widget2:
  title: "Did&aacute;ctico"
  url: 'http://comunidad-deepin.github.io/info/'
  text: '<em>Comunidad Deepin</em> ofrece contenido:<br/>1. Con imágenes de alta calidad.<br/>2. Vídeos en alta resolución.<br/>3. Compatible con dispositivos móviles.<br/>4. Fáciles de editar con <a href="http://commonmark.org/help/tutorial/">Markdown</a>.<br/>5. Y otras más...'
  video: '<a href="#" data-reveal-id="videoModal"><img src="http://comunidad-deepin.github.io/images/widget-2-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Rec&iacute;proco"
  url: 'http://comunidad-deepin.github.io/contact/'
  image: widget-3-302x182.jpg
  text: '<em>Comunidad Deepin</em> es atentida por humanos. No importa si has participado con anterioridad, son todos bienvenidos. ¿Quieres estar al día? <a href="https://comunidad-deepin.github.io/feed.xml">¡Suscríbete!</a> ¿Tienes alguna sugerencia? ¡Puedes contactarnos con nuestro equipo!'
#
# Use the call for action to show a button on the frontpage
#
# To make internal links, just use a permalink like this
# url: /getting-started/
#
# To style the button in different colors, use no value
# to use the main color or success, alert or secondary.
# To change colors see sass/_01_settings_colors.scss
#
callforaction:
  url: 'http://comunidad-deepin.github.io/instalacion'
  text: 'Descarga e instala la última versión de Deepin ›'
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---

<div id="videoModal" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/P7AdcIifRFY" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
