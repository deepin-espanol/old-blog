---
#
# Usamos los widgets y la cadena del contenido
# para incrustarlo automáticamente, si estás
# editando, revisa › layout: frontpage
#
# Nota: La base es http://deepin-espanol.github.io
#
layout: frontpage
teaser: "¡Una alternativa en nuestro idioma! Conoce Deepin, no solo por ser Linux. Te enseñamos a usarlo, cuidarlo y mantenerlo completo."
meta_teaser: "Una alternativa en nuestro idioma"
header:
  image_fullwidth: header_unsplash_12.jpg
# Widgets
widget1:
  title: "Instructivo"
  url: '/blog/'
  image: widget-1-302x182.jpg
  text: 'Llevamos el conocimiento para conocer y dominar nuestro software. <em>Deepin en Español</em> ofrece una <a href="/instalacion/">guía de instalación</a>, <a href="/manual/">serie de tutoriales</a> y <a href="/apps/">listados de aplicaciones</a>. Además, añadimos un blog de <a href="/noticias/">noticias</a> para estar al tanto de los últimos lanzamientos.'
widget2:
  title: "Did&aacute;ctico"
  url: '/info/'
  image: widget-2-302x182.jpg
  text: 'En <em>Deepin en Español</em> nos comprometemos:<br/>1. <a href="/tutopost/">Contenido enriquecido</a>.<br/>2. Ilustraciones y vídeos.<br/>3. Multiplataforma.<br/>4. Tips y <a href="/anexos/dudas/">dudas frecuentes</a>.<br/>5. Y otras más...'
widget3:
  title: "Rec&iacute;proco"
  url: '/actividades/'
  image: widget-3-302x182.jpg
  text: '<em>Nuestra comunidad</em> es atentida por humanos. No importa si has participado con anterioridad, son <a href="/actividades/">todos bienvenidos</a>. ¿Quieres estar al día? <a href="/feed.xml">¡Suscríbete!</a> ¿Tienes alguna sugerencia? ¡Puedes <a href="/info/contacto/">contactar</a> con nuestro equipo!'
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
  url: 'https://deepin-espanol.github.io/presentacion'
  text: 'Echa un vistazo a lo que ofrecemos ›'
  style: alert
permalink: /index.html
#
# This is a nasty hack to make the navigation highlight
# this page as active in the topbar navigation
#
homepage: true
---
