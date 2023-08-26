<ul style="list-style-type: none; padding: 0px;">
{% for post in site.posts %}

  {% unless page.unlisted %}
  <li style='margin-top: .5em;'>
    <b><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></b> - {{ post.description }}
    ({{ post.date | date: "%A, %B %e, %Y" }})
  </li>
  {% endif %}

{% endfor %}
</ul>