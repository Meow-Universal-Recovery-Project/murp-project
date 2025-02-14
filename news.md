---
layout: default
title: News
---
<div class="container mx-auto my-14">
<h1 class="text-5xl font-bold">News</h1>
<ul class="list-disc ml-10 my-2">
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | replace: '.html', '' }}">{{ post.title }}</a> [{{post.date | date: "%Y-%m-%d" }}]
    </li>
  {% endfor %}
</ul>
</div>
