---
layout: page
title: About
---
{% for French in site.tags %}
  <h3>{{ French }}</h3>
  <ul>
    {% for post in French %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}
