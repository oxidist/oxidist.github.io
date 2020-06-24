---
layout: default
---
<span style="font-variant:small-caps;">This is the website</span> of **Oxide**. I created this website to write about mathematics, linguistics, psychology, etc.

For more information about me, see [About]({{site.url}}/about).
# Recent
  {% for post in site.posts %}
  <article> 
    <p>
      <small><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></small>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </p>
  </article>
{% endfor %}

