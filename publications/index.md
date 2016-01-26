---
title: Publications
author: Roger Wong
layout: default
---
<div>
<h1 class="page-heading">Posts</h1>
<ul class="post-list" style="list-style-type:none">
  {% for post in site.posts %}
    {%if post.categories contains 'publications' %}
        <li>
          <h2>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          </h2>
          <p>{{post.content}}</p>
          <p>{{post.link}}</p>
        </li>
    {% endif %}
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>


</div>
