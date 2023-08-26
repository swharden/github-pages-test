this is the main page `index.md` file asdf

## Posts

<ul>
{% for post in site.posts %}
  <li class='margin-top: .5em;'><b><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></b> - {{ post.description }}</li>
{% endfor %}
</ul>

## Tags

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li class='margin-top: .5em;'><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
