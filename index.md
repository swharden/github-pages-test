this is the main page `index.md` file asdf

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.permalink }}">{{ post.title }}</a>
      <p>{{ post.description }}</p>
    </li>
  {% endfor %}
</ul>
