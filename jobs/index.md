---
id: 3659
title: Jobs
author: Modi Research Group
layout: default
guid: http://sel.columbia.edu/?page_id=3659
---
{% for post in site.categories.jobs %}
<div class="row-fluid">
    <div class="col-sm-12">
    <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
    </div>
</div>
{% endfor %}

<p class="rss-subscribe">subscribe <a href="{{ "/feed.xml" | prepend: site.baseurl }}">via RSS</a></p>
