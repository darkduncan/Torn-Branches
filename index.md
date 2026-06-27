---
layout: default
---

## Latest Posts

{% for post in site.posts limit:5 %}
  <div class="post-preview">
    <h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
    <p class="post-meta">{{ post.date | date: "%B %d, %Y" }}</p>
    <p>{{ post.excerpt | strip_html }}</p>
    <a href="{{ post.url | relative_url }}">Read more →</a>
  </div>
{% endfor %}

<p><a href="{{ site.baseurl }}/archive/">View all posts</a></p>
