# Advertencias de uso en la página Deepin en español.
Si te acostumbras a crear y editar posts, no es necesario que leas está página. Solo los administradores que están actualizando Jekyll deberán leer estas notas.

## Qué hemos modificado

Las diferencias con el tema de Jekyll Feeling Responsive son varias y están relacionados con la estética.

### Código modificado en layouts>frontapage

Si vas actualizar una parte del código debe conservarse como esto: 
´´´
{% comment %}
*
* EDITADO PARA MOSTRAR SOLO NOTICIAS
* Usando etiquetas
* site.categories.noticias
* category al final
* First check, if there are any posts at all
{% endcomment %}

{% unless site.categories.noticias == empty %}
    <div class="row t30 b20 homepage">
        <div class="small-12 columns">
            {% for post in site.categories.noticias limit:1 %}
            {% if post.image.homepage %}
            <p>
                <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ post.title | escape_once }}"><img width="970" src="{{ site.urlimg }}{{ post.image.homepage }}" alt="{{ page.title | escape_once }}"></a>
            </p>

            {% if post.image.caption_url and post.image.caption %}
            <p class="text-right caption">
                <a href="{{ post.image.caption_url }}">{{ post.image.caption }}</a>
            </p>
            {% endif %}
            {% else post.image.homepage == NULL %}
            <h2>{{ site.data.language.new_blog_entries }}</h2>
            {% endif %}
            {% endfor %}
        </div><!-- /.small-12.columns -->
    </div><!-- /.row -->


    <div class="row">
        <div class="medium-6 columns">
            {% for post in site.categories.noticias limit:1 %}
            {% if post.subheadline %}<p class="subheadline">{{ post.subheadline }}</p>{% endif %}
            <h2><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
            <p>
                {% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% else post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}
                <a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="Read {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
            </p>
            {% endfor %}
        </div><!-- /.medium-5.columns -->


        <div class="medium-6 columns">
            <p><strong>{{ site.data.language.more_articles }}</strong></p>
            {% include list-posts category='noticias' entries='3' offset='1' %}
        </div><!-- /.medium-7.columns -->
    </div><!-- /.row -->
{% endunless %}
´´´
Sirve para mostrar las noticias en la página de inicio.

### Otros detalles
Hay otro en sidebar.html en _includes y la carpeta de imágenes en assets, tampoco modifiques.

### Imágenes

Con el fin de hacer una página web más rápida recomendamos aligerar el peso de las imágenes sin sacrificar calidad. Ejemplos en la web son [tinypng](https://tinypng.com/) y [JPEGMini](http://www.jpegmini.com/main/shrink_photo).
