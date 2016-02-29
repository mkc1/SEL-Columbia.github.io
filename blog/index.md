---
title: Blog
layout: default
---

<div class="container">
    <strong>10 most recent posts</strong>
    <a href="/blog/archive">Blog archive</a>
    {% for post in site.categories.blog limit: 10 %}
        {% include post_summary.html post=post %}
    {% endfor %}
    <strong>10 most recent posts</strong>
    <a href="/blog/archive">Blog archive</a>
</div>
