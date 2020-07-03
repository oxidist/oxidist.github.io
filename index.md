---
layout: index
---
<span style="font-variant:small-caps;">This is the website</span> of **Oxide**. I write about mathematics, linguistics, computer science, etc.

For more information about me, see [About]({{site.url}}/about).
<section markdown="1">
# Recent
  <ul>
  {% for post in site.posts %}
      <li> <a href="{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  </ul>
</section>
