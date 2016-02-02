---
title: Blog
layout: default
---

<div class="container">
    {% for post in site.categories.blog limit: 8%}
        <div class="row">
            <h2>
                <a href="{{ post.url | prepend: site.baseurl }}">
                    {{ post.title }}
                </a>
            </h2>
            
            <p>
                <span class="article-author">
                    {{ post.author }}
                </span>
                <span class="article-date">
                    {{ post.date | date: "%b %-d, %Y"}}
                </span>
            </p>
            
            <p>
                {{ post.content | strip_html | truncatewords: 50 }}
            </p>
        </div>
    {% endfor %}
</div>
