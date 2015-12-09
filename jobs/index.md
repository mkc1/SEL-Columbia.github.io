---
id: 3659
title: jobs
author: Modi Research Group
layout: page
guid: http://sel.columbia.edu/?page_id=3659
---
<ul class="post-list">
  {% for post in site.posts %}
    {%if post.categories contains 'jobs' %}
        <li>
          <h2>
            <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
          </h2>
        </li>
    {% endif %}
  {% endfor %}
</ul>

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
