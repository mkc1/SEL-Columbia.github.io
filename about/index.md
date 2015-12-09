---
id: 27
title: About
author: John Humphrey
layout: default
guid: http://modilabs.org/?page_id=27
---

{% for post in site.categories.about %}

<div class="row">
  <div class="col-md-9 col-lg-6 col-sm-12"> 
    <h2>{{ post.title }}</h2>
    <p>{{ post.content }}</p> 
  </div>
</div>

{% endfor %}
