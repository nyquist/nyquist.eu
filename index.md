---
layout: page
title: Hello World!
tagline: Supporting tagline
---

# Recent posts
    
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

# Tags
{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}


