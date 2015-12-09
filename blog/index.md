---
id: 27
title: Blog
author: John Humphrey
layout: default
guid: http://modilabs.org/?page_id=27
---

<div class="container">
    {% for post in site.categories.blog limit: 8%}


    <div class="row">
        <article class="post-4547 post type-post status-publish format-standard hentry category-news">
          <header>
            <h2 style="margin-bottom: 0px !important; padding-bottom: 0px !important;">
                <a href="{{ post.url | prepend: site.baseurl }}" style="color: #000;">{{ post.title}} </a></h2>
                <p style="text-decoration: none !important; font-size: 14px;">
                   <span class="article-author"><a href="http://sel.columbia.edu/author/ssherpa/" title="Posts by Shaky Sherpa" rel="author">{{ post.author}}</a> </span>
                   <span class="article-date">{{ post.date | date: "%b %-d, %Y"}}</span></p>
               </header>

               <div>
                <a href="{{ post.url | prepend: site.baseurl }}">
                  <img class="first-image-thumbnail alignnone size-large wp-image-4513" src="http://sel.columbia.edu/wp-content/uploads/2015/05/Screenshot-2015-05-28-14.20.48-700x238.png" alt="Water Pump" width="700" height="238" /></a>
                  <br>
                  {{ post.content | strip_html | truncatewords: 50 }}
                  <br>
                  <a href="{{ post.url | prepend: site.baseurl }}" style="text-transform:uppercase; font-size: 13px; font-weight: 700;">Continue Reading »</a>
              </div>

          </article>
      </div>


      {% endfor %}
  </div>
