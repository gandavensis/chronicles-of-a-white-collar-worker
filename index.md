---
layout: home
title: Diary of a White Collar Worker
---

This is a public diary about work, routine, ambition, boredom, and everything in between.

{% for post in site.posts %}
<article>
  <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
  <p>{{ post.date | date: "%B %d, %Y" }}</p>
  {{ post.excerpt }}
</article>
{% endfor %}
