this is the main page `index.md` file asdf

## Posts

{% for post in site.posts %}
  <div>
    <a href="{{ post.url | absolute_url }}">{{ post.title }}</a> - {{ post.description }} 
  </div>
{% endfor %}

## Tags

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
