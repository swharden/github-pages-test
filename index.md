this is the main page `index.md` file asdf

<ul>
  {% for post in site.posts %}
    <div>
      <a href="{{ post.url }}">{{ post.title }}</a> - 
      {{ post.description }} 
      ({{ post.date | date: "%B %-d, %Y"  }})
    </div>
  {% endfor %}
</ul>
