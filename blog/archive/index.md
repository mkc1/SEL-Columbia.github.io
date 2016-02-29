---
title: Blog Archive
layout: default
---

<div class="container">
    <a href="/blog">Most recent posts</a>
    <strong>Blog archive</strong>
    {% for post in site.categories.blog %}
        <div class="row">
            <h2>
                <a href="{{ post.url }}">
                    {{ post.title }}
                </a>
            </h2>

            <p>
                <span class="article-author">
                    {% include author_name.html author=post.author %}
                </span>
                <span class="article-date">
                    {{ post.date | date: "%b %-d, %Y"}}
                </span>
            </p>
        </div>
    {% endfor %}
    <a href="/blog">Most recent posts</a>
    <strong>Blog archive</strong>
</div>
