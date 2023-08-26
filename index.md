this is the main page `index.md` file asdf

## Posts

<ul style="list-style-type: none;">
{% for post in site.posts %}
  <li class='margin-top: .5em;'><b><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></b> - {{ post.description }}</li>
{% endfor %}
</ul>

## Tags

{% for tag in site.tags %}
  <div>
    <b>{{ tag[0] }}:</b>
    {% for post in tag[1] %}
      <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>
    {% endfor %}
  </div>
{% endfor %}
