---
title: Blog
layout: default
---

<div class="container">
    <strong>10 most recent posts</strong>
    <a href="/blog/archive">Blog archive</a>
    {% for post in site.categories.blog limit: 10 %}
        <div class="row">
            <h2>
                <a href="{{ post.url }}">
                    {{ post.title }}
                </a>
            </h2>
            
            <p>
                <span class="article-author">
                    {% capture author_name %}{% include author_name.html author=post.author %}{% endcapture %}
                    {{ author_name }}
                </span>
                <span class="article-date">
                    {{ post.date | date: "%b %-d, %Y"}}
                </span>
            </p>

            {% comment %}
                http://stackoverflow.com/a/25466298/1475412
            {% endcomment %}
            {% assign images = post.content | split:"<img " %}
            {% for image in images %}
                {% if image contains 'src' %}
                    {% assign attributes = image | split:"/>" | first %}
                    <a href="{{ post.url }}">
                        <img {{attributes}} />
                    </a>
                    {% break %}
                {% endif %}
            {% endfor %}
            
            <br>
                {{ post.content | strip_html | truncatewords: 50 }}
            <br>
            <a href="{{ post.url }}" style="text-transform:uppercase; font-size: 13px; font-weight: 700;">Continue Reading &raquo;</a>
        </div>
    {% endfor %}
    <strong>10 most recent posts</strong>
    <a href="/blog/archive">Blog archive</a>
</div>
