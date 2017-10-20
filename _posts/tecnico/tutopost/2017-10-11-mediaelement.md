---
layout: page
subheadline: "Reproductor de música y vídeo"
title: "Añade vídeo y música a los post"
teaser: "¿Quieres añadir un podcast? ¿Quieres añadir un vídeo de Internet? Estás de suerte. Hemos integrado los post con <em>mediaelement.js</em>. Esa tecnología trabaja en todo navegador, incluido IE6-8."
tags:
    - tutopost
categories:
    - tecnico
breadcrumb: true
show_meta: false
header: no
image:
    title: mediaplayer_js-title.jpg
    thumb: mediaplayer_js-thumb.jpg
    homepage: mediaplayer_js-home.jpg
    caption: Foto por Corey Blaz
    caption_url: https://blaz.photography/
mediaplayer: true
---
{% include alert success='Esta página es un extracto de la serie de tutoriales, <a href="/tutopost">Tutopost</a>, para desarrollo en Jekyll' %}

[mediaelement.js][1] es para hacer magia. Su soporte es ideal para navegadores web. Para activar el reproductor de vídeo y audio tienes que añadir al encabezado y activarlo.

~~~
mediaplayer: true
~~~

Para incrustar la multimedia escribe el código HTML5...

{% highlight html %}
<audio src="http://path-to-file.com/music.mp3" type="audio/mp3" controls="controls"></audio>
{% endhighlight %}

Todas las funciones y cómo hacer *mediaelement.js* está completamente documentada en [su sitio web][1].

## »Music From All Around The World«

[»Music From All Around The World«][5] is a compilation curated by Jeannette Corneille and Moritz "mo." Sauer for [Phlow-Magazine.com][4]. Cover [Artwork designed by Jeannette Corneille][1]. All tracks were released under a [creative commons licence][2].

### B-Ju - »Philly Run«

<audio src="http://archive.org/download/music_from_all_around_the_world/13._music_from_all_around_the_world_-_b-ju_-_philly_run.mp3" type="audio/mp3" controls="controls"></audio>

### Comfort Fit - »Freeze The Cut«

<audio src="http://archive.org/download/music_from_all_around_the_world/05._music_from_all_around_the_world_-_comfort_fit_-_freeze_the_cut_opolopos_emotional_draft_remix.mp3" type="audio/mp3" controls="controls"></audio>

### The Black Atlantic - »Dandelion«

<audio src="http://archive.org/download/music_from_all_around_the_world/02._music_from_all_around_the_world_-_the_black_atlantic_-_dandelion.mp3" type="audio/mp3" controls="controls"></audio>

[Descargar compilación ›](https://archive.org/details/music_from_all_around_the_world)
{: .t30 .button .radius}



 [1]: http://mediaelementjs.com/
 [2]: http://jcorneille.de/
 [3]: www.creativecommons.org/licenses/by-nc-nd/3.0/
 [4]: http://phlow-magazine.com/
 [5]: https://archive.org/details/music_from_all_around_the_world
 [6]: #
 [7]: #
 [8]: #
 [9]: #
 [10]: #
