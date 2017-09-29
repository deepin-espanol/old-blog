---
#
# Usamos los widgets y la cadena del contenido
# para incrustarlo automáticamente, si estás
# editando, revisa › layout: frontpage
#
# Nota: La base es http://deepin-espanol.github.io
#
layout: frontpage
teaser: "¡Una alternativa en nuestro idioma!"
meta_teaser: "Una alternativa en nuestro idioma"
header:
  image_fullwidth: header_unsplash_12.jpg
# Widgets
widget1:
  title: "Instructivo"
  url: 'https://deepin-espanol.github.io/blog/'
  image: widget-1-302x182.jpg
  text: 'Llevamos el conocimiento para conocer y dominar nuestro software. <em>Deepin en Español</em> ofrece una guía de instalación, serie de tutoriales y listados de aplicaciones. Además, añadimos un blog de noticias para estar al tanto de los últimos lanzamientos.'
  video: '<a href="#" data-reveal-id="videoModal2"><img src="https://deepin-espanol.github.io/images/widget-1-302x182.jpg" width="302" height="182" alt=""/></a>'
widget2:
  title: "Did&aacute;ctico"
  url: 'https://deepin-espanol.github.io/info/'
  text: 'En <em>Deepin en Español</em> nos comprometemos:<br/>1. Contenido enriquecido.<br/>2. Ilustraciones y vídeos.<br/>3. Multiplataforma.<br/>4. <a href="/tutopost/">Publicaciones colaborativas</a>.<br/>5. Y otras más...'
  video: '<a href="#" data-reveal-id="videoModal"><img src="https://deepin-espanol.github.io/images/widget-2-302x182.jpg" width="302" height="182" alt=""/></a>'
widget3:
  title: "Rec&iacute;proco"
  url: 'https://deepin-espanol.github.io/contact/'
  image: widget-3-302x182.jpg
  text: '<em>Nuestra comunidad</em> es atentida por humanos. No importa si has participado con anterioridad, son todos bienvenidos. ¿Quieres estar al día? <a href="/feed.xml">¡Suscríbete!</a> ¿Tienes alguna sugerencia? ¡Puedes contactarnos con nuestro equipo!'
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
  url: 'https://deepin-espanol.github.io/download'
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
<div id="videoModal2" class="reveal-modal large" data-reveal="">
  <div class="flex-video widescreen vimeo" style="display: block;">
    <iframe width="1280" height="720" src="https://www.youtube.com/embed/dBAqsfE512g" frameborder="0" allowfullscreen></iframe>
  </div>
  <a class="close-reveal-modal">&#215;</a>
</div>
