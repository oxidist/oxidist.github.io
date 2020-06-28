---
layout: default
---
<span style="font-variant:small-caps;">This is the website</span> of **Oxide**. I created this website to write about mathematics, linguistics, computer science, etc.

For more information about me, see [About]({{site.url}}/about).
# <span style="font-variant:small-caps;">Recent</span>
<section>
  {% for post in site.posts %}
    <small><time datetime="{{ post.date | date: "%Y-%m-%d" }}">{{ post.date | date_to_long_string }}</time></small>
    <p>
      <a href="{{ post.url }}">
        {{ post.title }}
      </a>
    </p>
  {% endfor %}

</section>
