---
layout: default
title: Archive
---

<ul class="results">
  {% for post in site.posts %}
  <li>
    <header>
      <h1><a href="{{ post.url }}">{{ post.title }}</a></h1>
      <h2>{{ post.date | date: "%A %d, %B %Y" }}</h2>
      {% if post.comments != false %}
      <h3 class="comment-count"><a href="{{ post.url }}#disqus_thread" data-disqus-identifier="{{ post.url }}">Comments</a></h3>
      {% endif %}
      {% if post.tags != empty %}
      <ul class="tags">{% for tag in post.tags %}{{ tag }}
      <li></li>
      {% endfor %}
      </ul>
      {% endif %}
    </header>
  </li>
  {% endfor %}
</ul>
<script>
  var disqus_shortname = "k5han-blog";

  (function () {
    var s = document.createElement("script");
    s.async = true;
    s.src = "//" + disqus_shortname + ".disqus.com/count.js";

    document.getElementsByTagName("head")[0].appendChild(s);
  }());
</script>
