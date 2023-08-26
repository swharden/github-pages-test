<ul style="list-style-type: none; padding: 0px;">
{% for post in site.posts %}
  <li style='margin-top: .5em;'>
    <b><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></b> - {{ post.description }}
    ({{ post.date | date: "%A, %B %e, %Y" }})
  </li>
{% endfor %}
</ul>

{% for tag in site.tags %}
  <div style='margin-top: .5em;'>
    {{ tag[0] }}:
    {% for post in tag[1] %}
      <a href="{{ post.url | absolute_url }}">{{ post.title }}</a>,
    {% endfor %}
  </div>
{% endfor %}
